# Substrate-bug-fixing

`Error`: failed to run custom build command for `tikv-jemalloc-sys v0.4.3+5.2.1-patched.2` For fixing this error I found below command is very important:

```
cargo clean
rustup toolchain list
rustup uninstall nightly-2023-08-08-x86_64-unknown-linux-gnu
rustup uninstall nightly-x86_64-unknown-linux-gnu
rustup toolchain list
```
