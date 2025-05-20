# simple-home-dir
[![Crate](https://img.shields.io/crates/v/simple-home-dir.svg)](https://crates.io/crates/simple-home-dir)

**Deprecated**: This crate is no longer necessary as Rust now provides an official home_dir() method. Use `std::env::home_dir()` instead.

## Usage
Simply use the standard library's built-in [home_dir](https://doc.rust-lang.org/std/env/fn.home_dir.html) method.
```rust
pub use std::env::home_dir;

fn main() {
    // Unix     =>  /home/jdoe
    // Windows  =>  C:\Users\jdoe
    let path = home_dir().unwrap();
}
```