### go-gRPC-Test

#### PROTOC INSTALL
Download following link and add environment path
```bash
https://github.com/protocolbuffers/protobuf/releases/tag/v3.20.1
```

#### gRPC BUILD
```bash
protoc --go_out=./protos --go-grpc_out=./protos ./protos/*.proto
```

#### INSTALL
```bash
go get -d -v ./...
go install -v ./...
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go get google.golang.org/grpc
```

#### RUN
```bash
go run ./server/main.go
go run ./client/main.go
```