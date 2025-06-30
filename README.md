# 🔐 Vaultify – A Web3 Wallet

**Vaultify** is a modern, React-based Web3 wallet that allows users to securely generate and manage **Ethereum** and **Solana** wallets from a single seed phrase. It’s designed for simplicity, speed, and cross-chain compatibility — perfect for exploring the decentralized web (Web3) without relying on external wallet extensions.

---

Live Demo: https://vaultify-web3-vaulet.vercel.app/

---

## 🚀 Key Features

- 🔑 **12-word Mnemonic (Seed Phrase)** generation (BIP39 standard)
- 🔄 **HD Wallets**: Derive Ethereum & Solana addresses from same seed
- 🪙 **Ethereum (ETH)** & **Solana (SOL)** address generation
- 📋 **One-click Copy**: Copy wallet addresses & seed easily
- 🌐 **Built-in DApp Browser** for Web3 site interaction
- 🎨 Responsive UI with smooth transitions (Framer Motion)

---

## 🧭 User Flow

1. **Create Wallet**
   - User clicks “Generate Wallet”
   - App creates a secure 12-word seed phrase

2. **Wallet Address Generation**
   - From the seed, Ethereum & Solana addresses are derived
   - Both addresses are shown and copyable

3. **Import Wallet (if existing)**
   - User can enter existing seed phrase to restore wallets

4. **DApp Browser**
   - Built-in browser opens Web3 apps (like OpenSea, Uniswap)
   - App connects internally using wallet (no MetaMask needed)

---

## ⚙️ Tech Stack

- **Frontend**: React.js, Tailwind CSS
- **Crypto & Wallets**:
  - `bip39` – Mnemonic (seed phrase) generation
  - `ethers.js` – Ethereum wallet/address
  - `@solana/web3.js` – Solana wallet/address
  - `ed25519-hd-key` – For Solana key derivation
- **Animations**: Framer Motion
- **Deployment**: Vercel

---

## 🔒 Security

- All wallet logic runs client-side
- Seed phrase is never stored/sent to server
- Users must **manually save their seed phrase** to recover wallets

---

## 🛠️ Setup Instructions

```bash
git clone https://github.com/yourusername/vaultify-web3-wallet
cd vaultify-web3-wallet
npm install
npm run dev
