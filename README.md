### qmgo gridfs wrap

### usage see mgo gridfs

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
  f.Write([]byte(str))
  defer f.Close()

```
