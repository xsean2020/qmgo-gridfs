### qmgo gridfs wrap

usage see [mgo gridfs](https://pkg.go.dev/github.com/globalsign/mgo#GridFS)

--- 


```
  cli, err = qmgo.Open(context.Background(), cfg, o...)
  if err != nil {
     panic(err)
  }
  gfs := NewGridFS(cli,"fs")
  f, err := gfs.Create("race_info")
  if err != nil {
    panic(err)
  }
  defer f.Close()
  f.Write([]byte(str))
  

```
