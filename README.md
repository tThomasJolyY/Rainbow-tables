# Rainbow Table Attack

![University](https://img.shields.io/badge/University-Project-2F77DF?labelColor=679EEE&style=for-the-badge)
![Rust](https://img.shields.io/badge/Rust-black?style=for-the-badge&logo=Rust&logoColor=ffffff)

Rainbow table attack on SHA-3-256 in progress..

# Collaborater

* [Thanushan Pirabakaran](https://github.com/uvsq21919161)
* [Maya Santini](https://github.com/0kchak)
* [Theo Fratczack](https://github.com/Bynawers)

# Install

Cargo et Rust installation
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Dependencies
```
cargo build
```

# Commands

Generate a hash from a word
```
cargo run sha3 <password>
```

Generate Rainbow Table with the chosen parameters (constants.rs)
```
cargo run table
```

Start the attack with the chosen parameters (constants.rs)
```
cargo run attack
```

Check the performance of the reduction functions and the rainbow table
```
cargo run perf -t <type>
```
With theses types :
```
reduction
attack
table
```

Delete json file in data (all files with --all)
```
cargo run delete <--all / -a>
```

Unit test of SHA-3-256 functions
```
cargo test
```
