# 🚀 Neon EVM System Program Library Implementation

## 📝 Overview
This project showcases how to leverage Neon EVM’s System Program Library, enabling Solidity smart contracts to communicate directly with Solana’s native system program and enabling advanced cross-chain composability. 


## Prerequisites

- Node.js (v16 or higher)
- A Solana wallet with SOL for deployment
- A Metamask wallet with NEON and wSOL for Deployment.
- Basic understanding of Solana and Ethereum development.

## Project Structure

```                                 
├── contracts/                                     # Smart contract file
│   ├── LibSystemProgram.sol
│   ├── LibSystemData.sol
│   └── CallSystemProgram.sol
└── test/                                          # Deployment scripts
    └── composability/
    |    └── spl-token.test.js
    └── Readme.md                                  # Project documentation
```

### Features
- **Composability contracts:** Serves as the core contract for the System  Program Library.
- **Precompiles:** Serves as helper contracts for the composability contracts.

### Installation
```bash
# Initialize project
git clone https://github.com/Harshkumar62367/spl-token-library
pnpm init
```

### Configuration
1. Create `.env` file in the root folder:
```env
PRIVATE_KEY_OWNER=XYZ
PRIVATE_KEY_USER_1=XYZ
PRIVATE_KEY_USER_2=XYZ
PRIVATE_KEY_USER_3=XYZ
PRIVATE_KEY_SOLANA=XYZ
PRIVATE_KEY_SOLANA_2=XYZ
PRIVATE_KEY_SOLANA_3=XYZ
PRIVATE_KEY_SOLANA_4=XYZ
```


2. Run the below script to deploy the Meme Launchpad
```
npx hardhat test test/composability/spl-token.test.js --network neondevnet
```

## Deployed Contracts and Key Transactions

- **Deployer Address:** [`0xd12A585952dea511B17299D10B5059Cbd75fE64A`](https://neon-devnet.blockscout.com/address/0xd12A585952dea511B17299D10B5059Cbd75fE64A)
- **CallSPLTokenProgram Contract:** [`0x45FeA2119b88351099e12b2eD8170DDAe3413C84`](https://neon-devnet.blockscout.com/address/0x45FeA2119b88351099e12b2eD8170DDAe3413C84)
- **CallSystemProgram Contract:** [`0x75cb45597CA8986404dB62D64eb996D100b47f21`](https://neon-devnet.blockscout.com/address/0x75cb45597CA8986404dB62D64eb996D100b47f21)
- **CallAssociatedTokenProgram Contract:** [`0xF95c9225Fad9a0BE7ECf9B2521C8e2e047b0096C`](https://neon-devnet.blockscout.com/address/0xF95c9225Fad9a0BE7ECf9B2521C8e2e047b0096C)

