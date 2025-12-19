# VERICERT
VERICERT is an innovative web-based decentralized application (dApp) developed for the Blockchain and Application course at IIUM. It empowers university panels to issue tamper-proof digital certificates and enables employers to instantly verify their authenticity. Leveraging the Ethereum blockchain for secure record-keeping and IPFS for decentralized file storage, VERICERT ensures trust, transparency, and integrity in academic credential verification.

# Objectives
- **University Panel (Issuer)**: Securely upload and issue tamper-proof digital certificates.
- **Employer (Verifier)**: Instantly verify the authenticity of a candidate’s certificate using a unique Certificate ID.

# Key Features
- Authorized certificate issuance by universities.
- Decentralized certificate storage via IPFS (Pinata).
- Blockchain-based certificate verification using Ethereum smart contracts.
- Public verification through Certificate ID.
- Secure and user-friendly issuing interface.

# Technology Stack
- Smart Contract: Solidity (CertificateRegistry.sol)
- Blockchain Framework: Hardhat (local development network)
- Frontend: HTML, CSS, JavaScript
- Backend: Node.js + Express
- File Storage: IPFS via Pinata API
- Wallet Integration: MetaMask

# How to Run
1. Clone the Repository & Install dependencies
```bash
npm install
```
2. Start Hardhat local node npx hardhat node
3. Compile and deploy smart contract npx hardhat run scripts/deploy.js --network localhost
4. Run backend server node server/index.js
5. Open the Frontend
- Open index.html to verify certificates
- Open upload.html to upload certificate PDFs to IPFS
- Open issue.html to issue certificates on-chain

# Environment Variables
Create a .env file inside your /server folder and paste the following (replace with your real keys) :
```bash
PRIVATE_KEY=your_hardhat_wallet_private_key
PINATA_API_KEY=your_pinata_api_key
PINATA_API_SECRET=your_pinata_api_secret
```
