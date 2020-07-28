- Tried the library: https://docs.rs/tonic/0.3.1/tonic/

```sh
$ cargo run --bin helloworld-server
```

```sh
$ grpcurl -plaintext -import-path ./proto -proto helloworld.proto -d '{"name": "Tonic"}' [::]:50051 helloworld.Greeter/SayHello
```
