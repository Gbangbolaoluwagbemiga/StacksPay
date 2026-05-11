# StacksPay Protocol

StacksPay is a modern, decentralized bill-splitting application built on the **Stacks blockchain**. It provides a transparent and fun way to decide "who's paying" by letting a decentralized spinner wheel make the choice, with results recorded immutably on-chain.

![StacksPay Banner](https://payeer-alpha.vercel.app/logo.png)

## 🚀 Overview

StacksPay leverages Clarity smart contracts to ensure that every spin is verifiable and fair. Whether you're splitting a lunch bill or deciding who handles the next round, StacksPay brings blockchain transparency to social payments.

### Key Features

- **On-Chain Results**: Every winner is recorded on the Stacks blockchain via the `payeer` smart contract.
- **Stacks Wallet Integration**: Seamlessly connect using Leather, Xverse, or other Stacks-compatible wallets.
- **Dynamic Spinner**: A smooth, interactive UI that randomly selects a payer from the session.
- **Session History**: Track past winners directly from the contract state.

## 🛠 Tech Stack

- **Frontend**: [Next.js](https://nextjs.org/) (TypeScript, Tailwind CSS)
- **Smart Contracts**: [Clarity](https://clarity-lang.org/)
- **Blockchain**: [Stacks](https://stacks.co/)
- **Wallet Provider**: [@stacks/connect](https://www.npmjs.com/package/@stacks/connect)

## 📦 Project Structure

```text
├── backend/                # Clarity Smart Contracts
│   ├── contracts/          # .clar contract files
│   ├── settings/           # Network configurations (Mainnet, Testnet, Devnet)
│   └── Clarinet.toml       # Clarinet project configuration
├── frontend/               # Next.js Application
│   ├── src/app/            # App router components
│   ├── public/             # Static assets
│   └── tailwind.config.ts  # Styling configuration
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+)
- [Clarinet](https://github.com/hirosystems/clarinet) (for contract development)
- A Stacks Wallet (Leather or Xverse)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Gbangbolaoluwagbemiga/StacksPay.git
   cd StacksPay
   ```

2. **Frontend Setup**
   ```bash
   cd frontend
   npm install
   npm run dev
   ```

3. **Backend Setup**
   ```bash
   cd ../backend
   clarinet check
   ```

## 📜 Smart Contract

The core logic resides in `backend/contracts/payeer.clar`. It handles:
- Recording the winner of each spin.
- Storing a session counter.
- Providing read-only functions to fetch recent history.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

*Built with ❤️ on Stacks.*

<!-- minor update for PR -->
<!-- minor update for PR -->
<!-- minor update for PR -->
<!-- minor update for PR -->
<!-- minor update for PR -->