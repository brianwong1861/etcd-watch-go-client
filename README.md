## etcd Watch example using Go client

- start etcd - `docker run --rm --name etcd -p 2379:2379 gcr.io/etcd-development/etcd /usr/local/bin/etcd --listen-client-urls http://0.0.0.0:2379 --advertise-client-urls http://192.168.99.100:2379`
- run client code - `go run etcd_watch_go_client_v5.go -etcdHost=192.168.99.100:2379 -etcdWatchKey=mykey`
- check logs

![](etcd_watch_client_logs.JPG)