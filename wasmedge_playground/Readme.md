Steps done

1. Enable wasmedge on docker desktop
2. Install rust `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
3. Cloned Rust Examples from wasmedge `git clone git@github.com:second-state/rust-examples.git`
4. Tryed to build hello folder `cargo build --target wasm32-wasi --release`
5. was not working so installed wasm32-wasi `rustup target add wasm32-wasi` and tryied again
6. built it for docker `docker buildx build --platform wasi/wasm -t rust-example-hello .`
7. was not working, so i used `docker build -t rust-example-hello-marco:0.1 .`



https://github.com/deislabs/containerd-wasm-shims/blob/main/deployments/k3d/DockerSetup.md
https://github.com/deislabs/containerd-wasm-shims/issues/87