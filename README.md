# DAO Governance - Stellar Smart Contract

A decentralized autonomous organization (DAO) governance application built on the Stellar blockchain. Submit proposals, cast weighted votes, and execute governance decisions through a modern, intuitive web interface.

## 🌟 Features

- **Submit Proposals**: Create governance proposals with customizable parameters including voting periods and categories
- **Weighted Voting**: Cast votes with configurable vote power on active proposals
- **Execute Governance**: Execute approved proposals or veto using governance authority
- **Real-time Status**: Track active proposals and wallet connection status
- **Freighter Integration**: Seamless integration with Freighter wallet for secure transactions
- **Responsive Design**: Modern UI with dark theme and smooth animations

## 📸 Screenshots

### Homepage / Hero Section
![Homepage](https://res.cloudinary.com/dxkje9whm/image/upload/v1775590106/Screenshot_591_rsayti.png)

### Submit Proposal
![Submit Proposal](https://res.cloudinary.com/dxkje9whm/image/upload/v1775590105/Screenshot_592_r9tn5n.png)

### Vote Interface
![Vote Interface](https://res.cloudinary.com/dxkje9whm/image/upload/v1775590105/Screenshot_593_uxoege.png)

### Governance Actions
![Governance](https://res.cloudinary.com/dxkje9whm/image/upload/v1775590106/Screenshot_594_nqidv2.png)

## 🚀 Smart Contract

**Contract ID (Testnet):**
```
CA4VNQD74VJ3JIWGW32SIRCBLL4NHJQ2RZFPQABLDSAAPEAS3BN4FWOU
```

**View on Stellar Expert:**
https://stellar.expert/explorer/testnet/contract/CA4VNQD74VJ3JIWGW32SIRCBLL4NHJQ2RZFPQABLDSAAPEAS3BN4FWOU

## 🛠 Setup Instructions

### Prerequisites

- Node.js (v16 or higher)
- pnpm (recommended) or npm
- Freighter Wallet browser extension

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd stellar-dao-voting
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   ```
   
   Or with npm:
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   pnpm dev
   ```
   
   Or with npm:
   ```bash
   npm run dev
   ```

4. **Open in browser**
   - Navigate to `http://localhost:5173` (or the URL shown in terminal)
   - Install and configure Freighter wallet if you haven't already

### Building for Production

```bash
pnpm build
```

This creates an optimized production build in the `dist` folder.

## 📖 Usage

### 1. Connect Your Wallet

- Click "Connect Freighter" button
- Approve the connection in your Freighter wallet
- Your Stellar address will display at the top

### 2. Submit a Proposal

- Go to "Submit Proposal" tab
- Fill in proposal details:
  - **Proposal ID**: Unique identifier for proposal
  - **Title**: Proposal title
  - **Description**: Detailed description of the proposal
  - **Category**: Proposal category (e.g., treasury, protocol)
  - **Voting Period**: Duration in seconds (604800 = 7 days)
- Click "Submit Proposal"
- Approve transaction in Freighter

### 3. Cast Your Vote

- Navigate to "Vote" tab
- Enter proposal ID and your vote power
- Select position: **FOR** ✓ or **AGAINST** ✗
- Click "Cast Vote"
- Approve transaction in Freighter

### 4. Execute or Veto

- Go to "Governance Actions" tab
- Execute an approved proposal or veto using governance authority
- Provide executor/vetoer addresses as needed
- Approve transaction in Freighter

## 🔧 Technology Stack

- **Frontend**: React 19 with Vite
- **Blockchain**: Stellar SDK (`@stellar/stellar-sdk`)
- **Wallet**: Freighter API (`@stellar/freighter-api`)
- **Styling**: Custom CSS with CSS variables
- **Build Tool**: Vite

## 📦 Project Structure

```
stellar-dao-voting/
├── src/
│   ├── App.jsx              # Main application component
│   ├── App.css              # Application styles
│   ├── main.jsx             # React entry point
│   ├── index.css            # Global styles
│   └── lib/
│       └── stellar.js       # Stellar blockchain integration
├── public/                  # Static assets
├── screenshots/             # Screenshot directory
├── index.html              # HTML template
├── vite.config.js          # Vite configuration
├── eslint.config.js        # ESLint configuration
├── package.json            # Project dependencies
└── README.md               # This file
```

## 🔐 Security Notes

- Always verify contract addresses before interacting
- Ensure you're on the correct network (Testnet for development)
- Never share your private keys or seed phrases
- Use Freighter wallet for secure key management
- Test governance actions on testnet before mainnet deployment

## 🌐 Network Information

**Network**: Stellar Testnet  
**RPC URL**: `https://soroban-testnet.stellar.org`  
**Network Passphrase**: `Test SDF Network ; September 2015`

## 📄 Available Scripts

```bash
# Development server
pnpm dev

# Production build
pnpm build

# Preview production build locally
pnpm preview

# Lint code
pnpm lint
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## 📝 License

This project is open source and available under the MIT License.

## 🆘 Troubleshooting

### Wallet not connecting
- Ensure Freighter extension is installed
- Check that you're on the correct network (Testnet)
- Try refreshing the page and reconnecting

### Transaction fails
- Verify sufficient account balance
- Check contract ID is correct
- Review transaction details in Freighter for specific errors

### Slow transactions
- Wait for confirmation (may take a few seconds)
- Check Testnet status
- Verify RPC endpoint connectivity

## 📞 Support

For issues or questions, please open an issue on the repository or contact the development team.

---

Built with ❤️ for the Stellar community
