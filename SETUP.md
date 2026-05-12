# Setup Instructions - Reimagined Fishstick

## Prerequisites

- **Rust**: 1.70+ ([Install](https://rustup.rs/))
- **Cargo**: Comes with Rust
- **Git**: 2.0+
- **C/Clang compiler**: For C dependencies

### System Requirements

| OS | Version | Support |
|---|---|---|
| Linux | Ubuntu 20.04+ | ✅ Full |
| macOS | 11.0+ | ✅ Full |
| Windows | 10/11 | ✅ Full (WSL2 recommended) |

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/m74278803-cmyk/reimagined-fishstick.git
cd reimagined-fishstick
```

### 2. Install Dependencies

```bash
cargo build --release
```

### 3. Verify Installation

```bash
cargo test
```

## Development Setup

### Running in Debug Mode

```bash
cargo run
```

### Running Tests

```bash
# All tests
cargo test

# Specific test
cargo test test_parser

# With output
cargo test -- --nocapture
```

### Building Documentation

```bash
cargo doc --open
```

## Troubleshooting

### Issue: `rustc` not found
**Solution**: 
```bash
rustup update
rustup component add rustfmt
```

### Issue: Compilation timeout
**Solution**: Increase build timeout
```bash
CARGO_NET_GIT_FETCH_WITH_CLI=true cargo build --release
```

### Issue: Permission denied on macOS
**Solution**:
```bash
chmod +x target/release/reimagined-fishstick
```

## Common Commands

```bash
# Format code
cargo fmt

# Lint
cargo clippy

# Build
cargo build --release

# Run
cargo run --release

# Clean
cargo clean

# Dependencies update
cargo update
```

## Contributing

1. Create feature branch: `git checkout -b feature/your-feature`
2. Commit changes: `git commit -am 'Add feature'`
3. Push: `git push origin feature/your-feature`
4. Create Pull Request

## Documentation

- [Rust Guide](https://doc.rust-lang.org/)
- [Cargo Manual](https://doc.rust-lang.org/cargo/)
- Project docs: `cargo doc --open`

## Support

For issues, check:
1. [GitHub Issues](https://github.com/m74278803-cmyk/reimagined-fishstick/issues)
2. [Discussions](https://github.com/m74278803-cmyk/reimagined-fishstick/discussions)
