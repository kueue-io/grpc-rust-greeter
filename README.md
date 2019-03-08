### GRPC Rust Example

* GRPC rust example project for [grpc-rust](https://github.com/stepancheg/grpc-rust)
* Run generate cert script `gen-certs.sh` before run examples

#### Test client and server with Plain Text

```
# start greeter server implemented in rust
$ cargo run --bin greeter_server

# start greeter client implemented in rust
$ cargo run --bin greeter_client rust
> message: "Hello rust"
```

#### Test client and server with TLS

```
$ cargo run --bin greeter_server -- --tls
$ cargo run --bin greeter_client -- --tls
```
