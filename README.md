# 🌐 Soroban Token Contract on Futurenet

This project contains a Soroban smart contract deployed on the **Stellar Futurenet** test network.

---

## ✅ Contract Deployment  
The contract has been successfully deployed on Futurenet.

**Contract ID:**  
`CBLFZ33ACKB7A25277XKLU6F5R3NVQUQUXUTNRLFL4VVPAGQMSDOPG`

---

## 🧪 How to Interact

You can interact with this contract using:

- ✅ Soroban CLI tools  
- ✅ RPC requests (Stellar testnet RPC)
- ✅ Frontend dApp (optional)

Example CLI usage:

```bash
soroban contract invoke \
  --id CBLFZ33ACKB7A25277XKLU6F5R3NVQUQUXUTNRLFL4VVPAGQMSDOPG \
  --fn balance \
  --arg "ADDRESS_STRING_HERE"
```

---

## 📁 Project Structure

```bash
src/           # Contract source code (Rust)
Cargo.toml     # Rust dependency configuration
README.md      # Project description and deployment info
```

---

## 🛠 Technologies Used

- [Rust](https://www.rust-lang.org/)
- [Stellar Soroban SDK](https://soroban.stellar.org/)
- [Soroban CLI](https://docs.stellar.org/smart-contracts/soroban-cli)

---

## 🚀 Deployment Steps (Quick Reference)

```bash
soroban contract build
soroban contract deploy \
  --wasm target/wasm32-unknown-unknown/release/your_contract.wasm \
  --network futurenet
```

---

## 📬 Contact

Made by [@mykarli](https://github.com/mykarli) – feel free to reach out for collaboration!
