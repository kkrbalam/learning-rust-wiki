# Steps to Cross Compile from Linux to Windows

1. `rustup target add x86_64-pc-windows-gnu`
1. Add the file `config` into a new folder `.cargo` with the contents below
1. Install the package `mingw-w64` with the command `sudo apt install mingw-w64`
1. Compile with the command `cargo build --release --target x86_64-pc-windows-gnu`

## Config file

```
[target.i686-pc-windows-gnu]
linker = "i686-w64-mingw32-gcc"

[target.x86_64-pc-windows-gnu]
linker = "x86_64-w64-mingw32-gcc"
```