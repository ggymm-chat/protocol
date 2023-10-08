### 安装 buf

#### windows

安装 scoop

```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh -Proxy 'http://127.0.0.1:9910' | iex
```

使用 scoop 安装 buf

```bash
scoop config proxy '127.0.0.1:9910'
scoop install buf
```

#### 其他系统

参考 [buf 安装](https://buf.build/docs/installation)

### 安装 golang 库

```bash
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest

# 以下是可选的
go install github.com/envoyproxy/protoc-gen-validate@latest
go install github.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2@latest
go install github.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-grpc-gateway@latest
```

