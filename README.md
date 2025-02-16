# Quantum-Secured Bitcoin (QSB)

Quantum-Secured Bitcoin (QSB) is a blockchain project that aims to future-proof Bitcoin's security against quantum computing threats. It implements post-quantum cryptography (PQC) algorithms to replace traditional encryption and signature mechanisms, ensuring that the network remains secure even in the era of advanced quantum computing.

---

## Features

- **Post-Quantum Encryption**: Utilizes CRYSTALS-Kyber for encryption to protect transaction data from quantum attacks.
- **Quantum-Safe Signatures**: Replaces Bitcoin’s traditional ECDSA signatures with CRYSTALS-Dilithium to ensure transaction authenticity.
- **Secure Key Exchange**: Incorporates a simulated Quantum Key Distribution (QKD) protocol for secure key distribution.
- **Quantum-Resistant Consensus**: Uses Bitcoin’s Proof-of-Work (PoW) consensus with SHA-3 for enhanced quantum resistance.

---

## Technology Stack

- **Blockchain Core**: Bitcoin Core (modified)
- **Cryptography**: Open Quantum Safe (OQS) library for post-quantum encryption and signatures
- **Languages**: C++, Python
- **Development Environment**: Docker for environment setup and isolated testing
- **Web Interface**: Node.js and React for wallet and blockchain explorer

---

## Installation

### Prerequisites
- Docker installed on your system
- Git installed on your system

### Steps

1. Clone the QSB repository:
   ```bash
   git clone https://github.com/your-repo/qsb.git
   cd qsb
   ```
2. Build the modified Bitcoin Core:
   ```bash
   make
   ```
3. Run the blockchain node:
   ```bash
   ./bitcoind
   ```
4. Start the quantum-secure wallet:
   ```bash
   ./qsb-wallet
   ```

---

## Usage

1. **Starting the Node**: Run the QSB node using the above command.
2. **Generating Addresses**: Use the wallet to generate quantum-safe addresses for receiving transactions.
3. **Sending Transactions**: Transactions are signed and broadcast using CRYSTALS-Dilithium for maximum security.
4. **Monitoring the Blockchain**: Access the blockchain explorer interface for transaction and block details.

---

## Roadmap

### **Phase 1: Fork and Setup (Days 1–10)**
- Fork Bitcoin Core and set up a local blockchain testnet.
- Verify that the forked code runs without errors.

*Deliverable*: Functional Bitcoin fork running on a local testnet.

### **Phase 2: Integrate Quantum Cryptography (Days 11–20)**
- Replace ECDSA with CRYSTALS-Dilithium for quantum-safe signatures.
- Integrate CRYSTALS-Kyber for encryption and key exchange.
- Upgrade hash functions to SHA-3 for quantum resistance.

*Deliverable*: Transactions signed and verified using quantum-safe cryptography.

### **Phase 3: Wallet Development (Days 21–30)**
- Create a wallet that supports quantum-safe addresses and keys.
- Ensure wallet transactions remain compatible with the blockchain.

*Deliverable*: Fully functional quantum-secure wallet.

### **Phase 4: Testing and Security Audits (Days 31–35)**
- Comprehensive testing for quantum security and performance.
- Conduct penetration testing to identify vulnerabilities.

*Deliverable*: Tested, secure blockchain ready for deployment.

### **Phase 5: Testnet Deployment and Launch (Days 36–40)**
- Deploy QSB on a public testnet.
- Collect feedback and iterate on issues.
- Finalize all documentation.

*Deliverable*: Public testnet launch and complete project documentation.

---

## Security Considerations

- **Public Key Exposure**: Ensure transactions reveal the public key only after spending to minimize quantum attack risks.
- **Key Rotation**: Regularly rotate keys for enhanced security.
- **Community Audits**: Encourage public audits and feedback for ongoing improvements.

---

## Contributing

Contributions are welcome! Please follow the guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with detailed information on your changes.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments

- Bitcoin Core development team
- Open Quantum Safe (OQS) Project
- NIST Post-Quantum Cryptography Competition participants

---

