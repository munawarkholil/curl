# curl
esoftplay curl

# installation
1. clone repo
2. create class extends Esoftplay_Curl
3. override any function you want

# usage
  Methode GET => new Curl('uri',null,
                  (res,msg){
                    onDone
                  },
                  (msg){
                    onFailed
                  }
                )

  Methode POST => var post={
                    key1: 'value1',
                    key2: 2
                  }
                  new Curl('uri',post,
                    (res,msg){
                      onDone
                    },
                    (msg){
                      onFailed
                    }
                  )

  UPLOAD IMAGE/FILE =>  new Curl().upload('goal', 'image' ,fileUri, mimeType(def:'image/jpeg' if null),
                          (res,msg){
                            onDone
                          },
                          (msg){
                            onFailed
                          }
                        )
