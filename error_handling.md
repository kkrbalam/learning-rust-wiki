# Error Handling

Many ways to handle errors

[documentation](https://doc.rust-lang.org/std/result/)

Using the ? operator to handle errors in the main function so we don't have to write a match statement just to panic the code.

```rust
fn main() -> io::Result<()> { // the return statement is necessary
    let mut file = File::create("valuable_data.txt")?; // ? means if there is an error, panic
    file.write_all(b"important message")?;
    Ok(()) // this is what we are returning, it allows the ? to be used
}