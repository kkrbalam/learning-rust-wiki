# enums

This is an example of an enum that takes in an anonamous data structure, a new type, a type with a string value.

[documentation](https://doc.rust-lang.org/book/second-edition/ch06-01-defining-an-enum.html)
 
```rust
enum Command {
    Add {name: String, department: String},
    Get,
    GetByDepartment(String),
}
```