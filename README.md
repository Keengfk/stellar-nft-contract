# 🔗 Stellar NFT Contract

A Soroban smart contract for minting and managing Digital Art NFTs natively on the Stellar blockchain.

## 🌟 Overview

This contract replaces simple asset-based NFTs with a true on-chain smart contract — giving real ownership tracking, transfer logic, and metadata storage enforced by code rather than convention.

## ✨ Features

- 🎨 Mint NFTs with on-chain metadata (name, description, image URI)
- 👤 Track real ownership per token ID
- 💸 Transfer tokens with authorization checks
- 📊 Query total supply and token metadata

## 🛠️ Tech Stack

- **Language:** Rust
- **Platform:** Soroban (Stellar Smart Contracts)
- **Network:** Stellar Testnet

## 🚀 Getting Started

### Prerequisites
- Rust + Cargo
- `wasm32-unknown-unknown` target
- Stellar CLI

### Build

```bash
stellar contract build
```

### Deploy to Testnet

```bash
stellar contract deploy \
  --wasm target/wasm32-unknown-unknown/release/nft.wasm \
  --source <your-account> \
  --network testnet
```

## 📋 Contract Functions

| Function | Description |
|----------|-------------|
| `mint` | Mint a new NFT to an address with metadata |
| `owner_of` | Get the current owner of a token |
| `token_metadata` | Get name/description/image of a token |
| `transfer` | Transfer ownership of a token |
| `total_supply` | Get total tokens minted |

## 🔗 Related Project

This contract powers the NFT minting/transfer logic for [stellar-nft-app](https://github.com/Keengfk/stellar-nft-app), a React frontend for browsing and trading these NFTs.

## 📄 License

MIT License

## 👨‍💻 Author

**Keengfk** — Building NFT infrastructure for the Stellar ecosystem
