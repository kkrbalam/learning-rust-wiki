# Hash Map

## Methods that are useful

### entry

Entry is used to get a mutable reference to a value in the hashmap. It returns as an Option Some / Option None.

[documentation](https://doc.rust-lang.org/std/collections/hash_map/struct.HashMap.html#method.entry)

```rust
  let mut d = departments.entry(department);
  d.push(name);
```

### .or_insert

Or insert is used to insert new data into the hashmap in the case that the entry used previously didn't find any data. It will be what is returned if there was no original key.

[documentation](https://doc.rust-lang.org/std/collections/hash_map/enum.Entry.html)

```rust
  let mut d = departments.entry(department).or_insert(vec![]);
  d.push(name);
```