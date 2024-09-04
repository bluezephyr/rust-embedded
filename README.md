# Rust Embedded

## Documentation

* https://docs.rust-embedded.org/book/
* https://docs.rust-embedded.org/discovery/microbit/

## Hardware

https://tech.microbit.org/hardware/

## Host Toolchain

### Targets

Use `rustup target add <target-name>` to add support for targets in the build
tool chain. Check the `https://doc.rust-lang.org/nightly/rustc/platform-support.html` page for
details.

### LLVM Tools and Binutils

Install llvm-tools and cargo-binutils

```
rustup component add llvm-tools
cargo install cargo-binutils
```

Cargo binutils is a wrapper around llvm-tools for better ergonomics.

### Cargo Embed

Cargo embed is now part of probe-rs and is installed using

```
curl --proto '=https' --tlsv1.2 -LsSf https://github.com/probe-rs/probe-rs/releases/latest/download/probe-rs-tools-installer.sh | sh
```

To list attached probes, use the command `probe-rs list`

### Commands

```
cargo size -- -Ax
```

