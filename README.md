# 🖼️ NFT ERC-721 Project (Foundry)

This project implements two ERC-721 NFTs — `BasicNft` and `MoodNft` — using [Foundry](https://book.getfoundry.sh/) and leverages a `Makefile` to streamline testing, deployment, and development automation.

---

## ⚙️ Prerequisites

- [Foundry](https://book.getfoundry.sh/getting-started/installation.html)

```bash
curl -L https://foundry.paradigm.xyz | bash
foundryup
````

---

## 🧰 Setup & Installation

```bash
make install     # Install all dependencies (openzeppelin, foundry-std, foundry-devops)
make build       # Compile the smart contracts
```

---

## 🧪 Run Tests

### Local tests (Anvil):

```bash
make anvil       # Launch local test node
make test        # Run all tests
```

### ZkSync-compatible tests:

```bash
make zktest
```

---

## 🚀 Deployment & Interactions

Set your `.env` with the following values:

```env
SEPOLIA_RPC_URL=https://sepolia.infura.io/v3/YOUR_KEY
PRIVATE_KEY=your_deployer_private_key
ETHERSCAN_API_KEY=your_etherscan_api_key
```

### Deploy `BasicNft`

```bash
make deploy
```

### Mint `BasicNft`

```bash
make mint
```

### Deploy `MoodNft`

```bash
make deployMood
```

### Mint `MoodNft`

```bash
make mintMoodNft
```

### Flip Mood NFT State

```bash
make flipMoodNft
```

---

## ⚗️ Local ZkSync Deployment

Launch ZkSync-compatible deployment using:

```bash
make zkdeploy
```

---

## 🧹 Clean, Format, Snapshot

```bash
make clean      # Clean build files
make format     # Auto-format contracts
make snapshot   # Snapshot gas usage
```

---

## 📜 License

MIT License

---

Made with 🦄 using Foundry & Make.
