## udp server
```swift

udpsocket = udpbind("0.0.0.0",9090)
print("bound")
coroutine "main"{
    rec = udplisten(udpsocket)
    // rec !
    if rec[0] != ""{
        print(rec[0])
    }
    if len(rec) > 1{
        i ++
        print(rec[1])
        udpreply(udpsocket,rec[0],cat("ok",i))
    }
}```
