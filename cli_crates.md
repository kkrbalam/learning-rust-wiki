# Crates and their usage

** From Felix **

For command-line parsing in larger CLI apps, you can use [structopt](https://crates.io/crates/structopt) or [clap](https://crates.io/crates/clap) (which structopt builds on). Because you generally want to immediately return if the passed arguments aren't correct, it makes sense to just parse-and-unwrap-on-error, but these tools can do things such as auto-generate --help flags, do fuzzy matching (i.e. "you typed --hlp, did you mean --help?"), conditional arguments, coloring of console output, etc. 