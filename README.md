# 🎨 Challenge 0 - Simple NFT Example (Speedrun Ethereum)

This project was developed as part of the **[Discovery Basecamp](https://speedrunethereum.com/)** program, following the Speedrun Ethereum Challenge 0. It consists of deploying an ERC721 (NFT) smart contract to the Sepolia network, interacting with it through a frontend app, and publishing it with a user-friendly interface on Vercel.

---

## 🚀 Technologies Used

- Scaffold-ETH 2
- Hardhat + Solidity
- Sepolia Testnet
- Alchemy
- MetaMask
- Etherscan
- Vercel

---

## ✅ Steps Completed

### 1. Create the base project
```bash
npx create-eth@0.1.0 -e challenge-0-simple-nft challenge-0-simple-nft
cd challenge-0-simple-nft
```
Start local chain in a separate terminal:
```bash
yarn chain
```
Deploy contracts locally:
```bash
yarn deploy
```
Start the frontend:
```bash
yarn start
```

### 2. Generate a local development wallet
```bash
yarn generate
```
This creates an address to be used for contract deployment via Hardhat.

### 3. Fund the wallet
- SepoliaETH was obtained from a faucet and sent to the generated deployer address.

### 4. Deploy the NFT contract `YourCollectible` to Sepolia
```bash
yarn deploy --network sepolia
```
Deployed contract address:
```
0xB12a31c107603a6D657f82571008b71FAecc8389
```

### 5. Verify the contract on Etherscan
```bash
yarn verify --network sepolia
```
Result: successfully verified.

🔗 [View on Sepolia Etherscan](https://sepolia.etherscan.io/address/0xB12a31c107603a6D657f82571008b71FAecc8389)

### 6. Run frontend locally
```bash
yarn dev
```
Opened at: `http://localhost:3000`

Connected to MetaMask (on Sepolia), used the `mintItem()` function to mint NFTs.

---

## 🌐 Deployed frontend on Vercel

Frontend was deployed using:
```bash
yarn vercel
```

🔗 [Live App on Vercel](https://nft-project-saudlari-larissas-projects-6fce7247.vercel.app/)

---

## 🔐 API Keys Used (optional but recommended)

### Alchemy
- A project was created in the Alchemy dashboard for Sepolia.
- Keys stored in `.env` and `.env.local`:
```env
ALCHEMY_API_KEY=...
NEXT_PUBLIC_ALCHEMY_API_KEY=...
```

### Etherscan
- API key obtained from [Etherscan API](https://etherscan.io/) and stored in:
```env
ETHERSCAN_API_KEY=...
```

---

## 🎉 Result

- ✅ Contract deployed and verified on Sepolia
- ✅ Frontend working on Vercel
- ✅ NFT successfully minted from UI
- ✅ Challenge 0 submitted successfully

---
