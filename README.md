# sn

## build

```sh
# build debug
cargo build

# build release
cargo build --release

# build sn release
cargo build --release --bin sn

# cross build 
# 1. add .cargo/config.toml
[target.aarch64-unknown-linux-gnu]
linker = "xxx/aarch64-none-linux-gnu-gcc"
# 2. export CC and build
export CC="xxx/aarch64-none-linux-gnu-gcc"
cargo build --release --target aarch64-unknown-linux-gnu
```
