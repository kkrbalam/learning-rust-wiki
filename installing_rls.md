# Installing RLS

## VS Code

### Linux

* VS Code will attempt to install the appropriate components to rustup, but might fail. If it does, then run this command to install them manually.

```bash
rustup component add rls-preview rust-src rust-analysis
```