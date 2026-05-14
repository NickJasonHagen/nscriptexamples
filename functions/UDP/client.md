## udp client
```swift

udpsocket = udpbind("127.0.0.1",9091)
server = socketaddress("0.0.0.0",9090)
coroutine "main"{
    i ++
    udpsend(udpsocket,server,cat("hellow",i))
    rec = udplisten(udpsocket)
    if len(rec) > 1{
        print(rec[1])
    }
}```
