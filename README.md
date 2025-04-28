# A-Blockchain-Based-E-Voting-System-Using-Hyperledger-Fabric
Overview
This project is a secure, decentralized e-voting system built using:

Hyperledger Fabric for blockchain infrastructure

React.js frontend for a seamless user experience

Node.js/Express.js backend for handling APIs

MongoDB for secure voter metadata storage

IPFS for encrypted ballot storage

Zero-Knowledge Proofs (ZKP) for voter privacy and eligibility verification

The system is designed to ensure voter anonymity, vote integrity, tamper-resistance, and full verifiability.

🏗️ Project Architecture
Frontend (React.js):

Voter Login (MFA + OTP verification)

Voting Dashboard

Admin Panel for Result Visualization

Backend (Node.js + Express.js):

Secure API communication with frontend

Voter authentication using JWT

OTP generation and validation

Interacts with Hyperledger Fabric Smart Contracts

Blockchain Layer (Hyperledger Fabric):

Stores IPFS hashes for vote verification

Executes Smart Contract (Chaincode) for vote validation

Storage Layer:

MongoDB: Stores voter registration metadata (encrypted)

IPFS: Stores encrypted ballots off-chain

Security Modules:

Zero-Knowledge Proofs for privacy-preserving authentication

HTTPS and token-based session security

⚙️ Installation Instructions
Prerequisites
Node.js and npm installed

MongoDB installed or MongoDB Atlas account

Docker and Docker-Compose (for Hyperledger Fabric)

IPFS node (optional, or public IPFS gateways)

Setup Steps
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/blockchain-e-voting-system.git
cd blockchain-e-voting-system
Install backend dependencies:

bash
Copy
Edit
cd backend
npm install
Install frontend dependencies:

bash
Copy
Edit
cd ../frontend
npm install
Start MongoDB:

bash
Copy
Edit
mongod
Run Hyperledger Fabric network:

bash
Copy
Edit
cd ../fabric-network
./startFabric.sh
Run Backend Server:

bash
Copy
Edit
cd ../backend
npm start
Run Frontend Client:

bash
Copy
Edit
cd ../frontend
npm start
Access Application:

Open browser and navigate to http://localhost:3000/

🚀 Features
Voter login with with MFA

Secure login with(Password + OTP)

Zero-Knowledge Proof verification for voter eligibility

Encrypted vote storage on IPFS

Immutable IPFS hash recording on Hyperledger Fabric

Real-time voting results visualization

End-to-end encryption and session security

📸 Screenshots
(Insert screenshots of the login page, voting dashboard, admin result dashboard, and blockchain transaction viewer.)

🛡️ Security Measures
HTTPS secure communication

Token-based authentication with JWT

Multi-Factor Authentication (MFA)

IPFS + Blockchain hybrid storage

Privacy-preserving ZKP verification

Audit logs for administrative actions

📚 References
This project implementation is based on:

Hyperledger Fabric documentation

IPFS public APIs

ZKP cryptographic libraries

Research studies on blockchain-based e-voting systems

