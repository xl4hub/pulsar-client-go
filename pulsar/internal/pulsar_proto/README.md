

```
go get github.com/gogo/protobuf/protoc-gen-gogofast
go get github.com/gogo/protobuf/proto
go get github.com/gogo/protobuf/gogoproto
go install github.com/gogo/protobuf/protoc-gen-gogofast
go install github.com/gogo/protobuf/proto
go install github.com/gogo/protobuf/gogoproto
```

Generate code:

```
protoc -I=. -I=$GOPATH/src -I=$GOPATH/src/github.com/gogo/protobuf/protobuf --gogofast_out=. PulsarApi.proto
```
