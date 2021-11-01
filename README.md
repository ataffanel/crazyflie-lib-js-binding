# Crazyflie lib WASM javascript binding

Javascript binding for the Rust-implemented [crazyflie-lib]. It compiles to
WASM with Javascript binding. It runs in a web-browser using webUSB  to access
the Crazyradio radio USB dongle. In the future NodeJS support can be added
either as a native node extension or using WASM and a webUSB implementation
for Node.

This lib is very much work in progress. The aim is to follow the state of the
[crazyflie-lib] Rust crate.

## Compiling

Compiling this crate requires [rust] and [wasm-pack]. Can be built with:

```
wasm-pack build
```

The resulting npm package will be in the `pkg` folder.


[crazyflie-lib]: https://github.com/ataffanel/crazyflie-lib-rs
[wasm-pack]: https://rustwasm.github.io/wasm-pack/installer/
[rust]: https://rustup.rs