

# 🌱 SeedVerse – Setup & Run Guide

**SeedVerse** is a decentralized application (dApp) that integrates blockchain technology with a web-based frontend, allowing users to interact with smart contracts seamlessly. Built with Next.js, Tailwind CSS, Hardhat, and Solidity, it offers a modern interface for blockchain interactions.

---

## 📦 Prerequisites

Before setting up the project locally, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)
- [Hardhat](https://hardhat.org/) – Ethereum development environment
- [MetaMask](https://metamask.io/) – Browser extension for Ethereum wallet

---

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/AryanS-88/SeedVerse.git
cd SeedVerse
```

---

### 2. Install Dependencies

```bash
npm install
```

---


---

### 3. Compile Smart Contracts

Navigate to the root directory and run:

```bash
npx hardhat compile
```

This will compile the Solidity contracts located in the `contracts/` directory.

---

### 4. Deploy Smart Contracts

To deploy contracts to a local Hardhat network:

```bash
npx hardhat node
```

In a new terminal window, deploy the contracts:

```bash
npx hardhat run scripts/deploy.js --network localhost
```

Note the deployed contract addresses for frontend integration.

---

### 5. Run the Frontend

Start the Next.js development server:

```bash
npm run dev
```

The application will be accessible at [http://localhost:3000](http://localhost:3000).

---

## 🧪 Testing

To run tests for the smart contracts:

```bash
npx hardhat test
```

---

## 📁 Project Structure

```plaintext
SeedVerse/
├── components/       # Reusable React components
├── contracts/        # Solidity smart contracts
├── context/          # React context for state management
├── pages/            # Next.js pages
├── public/           # Static assets
├── scripts/          # Deployment scripts
├── styles/           # Global styles
├── test/             # Contract tests
├── .env              # Environment variables
├── hardhat.config.js # Hardhat configuration
└── package.json      # Project metadata and scripts
```

---

## 📬 Support

For issues or feature requests, please open an [issue](https://github.com/AryanS-88/SeedVerse/issues) on the GitHub repository.

---
