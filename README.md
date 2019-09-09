# redisc
A Go redis client built on top of redigo.

Installation
------------

Install Redigo using the "go get" command:

    go get github.com/lufred/redisc
    
Example
------------
```
    err:=redisc.RegisterDb("",DriverRedis,"127.0.0.1:6380","")
    if err!=nil{
      t.Errorf("open err =%s",err.Error())
    }else{
      t.Log("open success")
    }
    cache,err:=redisc.GetCache("default)
    if err!=nil{
      fmt.Error(err)
    }
    cache.SSet("prefix","key","val",30)
```
   
   


