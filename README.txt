tutorial...
https://www.youtube.com/watch?v=Y92WWaZJl24

build...
protoc --proto_path=proto --proto_path=third_party --go_out=plugins=grpc:proto service.proto

run...
go run server/main.go &
go run client/main.go &

test...
http://localhost:8088/mult/22341421/3124124124
NOTE: I have used port 8088 not 8080 as in the tutorial because I was already using port 8080
(this is set at the bottom of client/main.go)