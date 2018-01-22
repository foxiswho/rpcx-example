# rpcx-example
golang  rpcx example

# 框架安装
## 服务发现注册 consul 安装
请打开连接查看，只看安装部分
http://blog.csdn.net/fenglailea/article/details/79093848

## 服务发现注册 consul docker 集群安装
请打开连接查看，一定要安装
http://blog.csdn.net/fenglailea/article/details/79098246

## 下载 rpcx 框架
```SHELL
go get -u -v -tags "reuseport quic kcp zookeeper etcd consul ping" github.com/smallnest/rpcx/...
```

## 下载 rpcx 案例 （不是必须）
这里的 rpcx 案例，是让你熟悉使用  rpcx 这个微服务框架
```SHELL
go get -v github.com/rpcx-ecosystem/rpcx-examples3
```
> 如果 goLang 类库下载错误，请在 http://blog.csdn.net/fenglailea/article/details/79107124 连接中，`Golang类库 下载` 解决

完成后，到你的`$GOPATH/src/github.com/rpcx-ecosystem/rpcx-examples3`目录下，进行案例 使用操作.

> 在使用 registry 目录下 server.go 时，直接 编译是不能通过的，需要加参数`-tags consul`,例如：`go run -tags consul server.go`或`go build -tags consul server.go`