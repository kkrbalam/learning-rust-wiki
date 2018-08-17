# Printing Values

## Debug

`#[derive(Debug)]`
Adding the ability to print with println! macro on data structures like enums, HashMaps, and Vectors.

[trait debug documentation](https://doc.rust-lang.org/std/fmt/trait.Debug.html)

### Example

```rust
#[derive(Debug)]
enum Command {
    Add {name: String, department: String},
    Get,
    GetByDepartment(String),
}
```

Now we can print with println!

```rust
println!("{:?}", our_enum);
```

## Printing to standard out

`eprintln!("this will go to standard out");`

[documentation](https://doc.rust-lang.org/std/macro.eprint.html)