# 🤝 Contributing to OrbitNFT

Thank you for your interest in contributing to OrbitNFT! This guide will help you get started.

## 📋 Prerequisites

Before you begin, make sure you have the following installed:

- [Rust](https://www.rust-lang.org/tools/install) (latest stable)
- [Soroban CLI](https://soroban.stellar.org/docs/getting-started/setup)
- [Node.js](https://nodejs.org/) (v18 or higher)

## 🛠️ Local Setup

### 1. Clone the repository
```bash
git clone https://github.com/Keengfk/stellar-nft-contract.git
cd stellar-nft-contract
```

### 2. Install the correct build target
```bash
rustup target add wasm32v1-none
```

### 3. Build the contract
```bash
cargo build --target wasm32v1-none --release
```

### 4. Run tests
```bash
cargo test
```

### 5. Deploy to Stellar Testnet
```bash
soroban contract deploy \
  --wasm target/wasm32v1-none/release/orbitnft.wasm \
  --network testnet
```

## 🌿 Branching

- `main` — stable, production-ready code
- `feat/your-feature-name` — new features
- `fix/your-fix-name` — bug fixes

## 📝 Pull Request Process

1. Fork the repository
2. Create a new branch from `main`
3. Make your changes
4. Run tests and make sure they pass
5. Submit a Pull Request with a clear description of your changes
6. Reference any related Issue in your PR description (e.g. `Closes #5`)

## 🐛 Reporting Bugs

Open an [Issue](https://github.com/Keengfk/stellar-nft-contract/issues) and include:
- What you expected to happen
- What actually happened
- Steps to reproduce

## 💡 Suggesting Features

Open an [Issue](https://github.com/Keengfk/stellar-nft-contract/issues) with the `enhancement` label and describe your idea clearly.

## 📄 Code Style

- Follow standard Rust formatting: run `cargo fmt` before committing
- Run `cargo clippy` and fix any warnings before submitting a PR

## 🏆 Recognition

All contributors will be listed in the README. Thank you for helping build OrbitNFT!
