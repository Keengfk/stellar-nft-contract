# 🔗 Stellar NFT Contract

A Soroban smart contract for minting and managing Digital Art NFTs natively on the Stellar blockchain.

## 🚀 Live Deployment

This contract is deployed and live on Stellar Testnet:

- **Contract ID:** `CD52JXC6QBQACDJGPPPZ6OWBJZ32SVJECYLKTU2WKBVO5NO7WVQNUCTR`
- **Explorer:** [View on Stellar Expert](https://stellar.expert/explorer/testnet/contract/CD52JXC6QBQACDJGPPPZ6OWBJZ32SVJECYLKTU2WKBVO5NO7WVQNUCTR)
- **First mint transaction:** [View on Stellar Expert](https://stellar.expert/explorer/testnet/tx/622d23550395c05dc47fc08e8d555115a9eb1ed0cd7011d50f210e67554f9dbf)
- **Status:** ✅ Builds successfully · ✅ All unit tests passing · ✅ Live mint confirmed

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
- `wasm32v1-none` target
- Stellar CLI

### Build
stellar contract build


### Deploy to Testnet
stellar contract deploy
--wasm target/wasm32v1-none/release/nft.wasm
--source <your-account>
--network testnet


## 📋 Contract Functions

| Function         | Description                                |
| ---------------- | ------------------------------------------ |
| `mint`           | Mint a new NFT to an address with metadata |
| `owner_of`       | Get the current owner of a token           |
| `token_metadata` | Get name/description/image of a token      |
| `transfer`       | Transfer ownership of a token              |
| `total_supply`   | Get total tokens minted                    |

## 🔗 Related Project

This contract powers the NFT minting/transfer logic for [stellar-nft-app](https://github.com/Keengfk/stellar-nft-app), a React frontend for browsing and trading these NFTs.

## 📄 License

MIT License

## 👨‍💻 Author

**Keengfk** — Building NFT infrastructure for the Stellar ecosystem
Commit it with a message like "Update README
