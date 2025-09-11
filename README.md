## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Somnia Test ( STT ) for gas fees
- Private keys for your wallets

## Installation

1. Clone the repository:
```bash
git clone https://github.com/rekajunardi/Somnia-Auto-TF.git
cd Somnia-Auto-TF
```

2. Install dependencies:
```bash
npm install
```

4. Configure your environment variables in `.env`:
```env
PRIVATE_KEY_1=your_first_private_key_here
PRIVATE_KEY_2=your_second_private_key_here
PRIVATE_KEY_3=your_third_private_key_here
# Add more private keys as needed (PRIVATE_KEY_4, PRIVATE_KEY_5, etc.)
```

## Usage

1. Start the bot:
```bash
npm start
```

2. The bot will:
   - Display all wallet information and balances
   - Ask for the number of transactions per wallet
   - Execute the configured transactions
   - Wait 24 hours before the next batch

## Configuration

### Environment Variables

- `PRIVATE_KEY_1`, `PRIVATE_KEY_2`, etc.: Your wallet private keys
- The bot automatically detects all private keys following the `PRIVATE_KEY_X` pattern

## Safety & Security

⚠️ **Important Security Notes:**

- Never share your private keys
- Only use testnet funds
- Keep your `.env` file secure and never commit it to version control
- This bot is for educational and testing purposes only

## Troubleshooting

### Common Issues

1. **"No valid private keys found"**
   - Check your `.env` file format
   - Ensure private keys are valid hex strings
   - Make sure private keys start with `0x` or are 64 characters long

2. **"RPC connection failed"**
   - Check your internet connection
   - The RPC endpoint might be down, try again later

3. **"Transaction failed"**
   - Insufficient balance for gas fees
   - Network congestion

   - Invalid transaction parameters
