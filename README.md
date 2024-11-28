# De-Polls
Decentralized Polling dApp
Overview
A Web3 decentralized polling application that allows users to create, vote on, and view poll results using Ethereum blockchain technology.
Features

Create polls with 2-4 options
Vote on active polls
View poll results
Prevents duplicate voting
MetaMask wallet integration

Prerequisites

Node.js (v14+ recommended)
MetaMask browser extension
Hardhat
React.js

Installation
1. Clone the Repository
bashCopygit clone https://github.com/yourusername/decentralized-polling.git
cd decentralized-polling
2. Install Dependencies
bashCopynpm install
3. Compile Smart Contracts
bashCopynpx hardhat compile
4. Run Local Blockchain
bashCopynpx hardhat node
5. Deploy Contract
bashCopynpx hardhat run scripts/deploy.js --network localhost
6. Start Frontend
bashCopynpm start
Environment Variables
Create a .env file in the project root with:
CopyREACT_APP_CONTRACT_ADDRESS=your_deployed_contract_address
REACT_APP_NETWORK_ID=your_network_id
Testing
bashCopynpx hardhat test
Deployment
For testnet deployment (e.g., Goerli):

Update hardhat.config.js with network details
Fund your deployment wallet with testnet ETH
Run npx hardhat run scripts/deploy.js --network goerli

Technologies

Solidity
React.js
Ethers.js
Hardhat
MetaMask

Security Considerations

Contract prevents duplicate voting
Validates poll creation parameters
Restricts voting to active polls
