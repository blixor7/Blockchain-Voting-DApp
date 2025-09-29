# Blockchain Voting DApp

A decentralized voting application built on Ethereum that brings transparency and security to electoral processes using blockchain technology.

## Overview

Traditional Electronic Voting Machines (EVMs) are susceptible to various forms of fraud and manipulation. This Blockchain Voting DApp leverages Ethereum smart contracts to create a tamper-proof, transparent voting system where votes are publicly verifiable while maintaining voter privacy.

## Tech Stack

- **Frontend**: React.js
- **Blockchain**: Ethereum
- **Smart Contracts** : Solidity
- **Web3 Integration**: Web3.js
- **Development**: Truffle Suite
- **Testing**: Ganache CLI

## Key Features

- **Secure Candidate Registration** - Contract owner can register candidates with names and addresses
- **One-Vote-Per-Voter** - Blockchain ensures each address can vote only once
- **Real-time Results** - View leading candidates and live vote counts
- **Transparent Process** - All votes ar recorded on the blockchain for public verification
- **Voter Privacy** - Votes are anonymous while maintaining auditability

## Quick Start

### Prerequisites

- Node.js (v14 or higher)
- MetaMask browser extension
- Ganache CLI or GUI

### Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/0xPleiades/Voting-Dapp.git
   cd Voting-Dapp
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Configure MetaMask**
   - Install MetaMask from [metamask.io](https://metamask.io/)
   - Choose "Import Wallet" and use Ganache's seed phrase
   - Add local network: `http://localhost:7545` with Chain ID `1337`
   - Import all test accounts from Ganache

4. **Deploy Smart Contracts**
   ```bash
   truffle migrate --reset
   ```

5. **Start the Application**
   ```bash
   npm start
   ```

## Project Structure

```
Voting-Dapp/
├── build/contracts/          # Compiled contract artifacts
├── client/                   # React frontend application
├── contracts/                # Solidity smart contracts
│   └── Election.sol         # Main voting contract
├── migrations/               # Deployment scripts
├── test/                    # Smart contract tests
├── truffle-config.js        # Truffle configuration
└── package.json            # Project dependencies
```

## How It Works

### For Contract Owners:
1. Deploy the voting contract
2. Register candidates with their details
3. Monitor voting process in real-time

### For Voters:
1. Connect MetaMask wallet
2. Browse registered candidates
3. Cast your vote (one-time only)
4. View live election results

## Security Features

- **Immutable Voting Records** - Once cast, votes cannot be altered
- **Prevention of Double Voting** - Smart contract logic prevents multiple votes
- **Transparent Tallying** - Vote counts are publicly verifiable
- **Anonymous Voting** - Voter identities are protected

## Testing

Run the test suite to verify contract functionality:

```bash
truffle test
```

## Live Demo

The application runs on `http://localhost:3000` after starting the development server.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## License

This project is licensed under the MIT License.

---
