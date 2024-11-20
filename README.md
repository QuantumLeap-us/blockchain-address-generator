## BLOCKCHAIN ADDRESS GENERATOR

A simple command-line tool to generate multiple wallet addresses for different blockchain networks.

## Features

- Generate multiple wallet addresses at once
- Support for multiple networks:
- EVM (Ethereum, BSC, Polygon, etc.)
- Solana
- Automatic wallet storage in JSON format
- User-friendly command-line interface
- Colored output for better readability

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Rambeboy/blockchain-address-generator.git
   ```

3. Navigate to the project directory:
   ```bash
   cd blockchain-address-generator
   ```

5. Install dependencies:
   ```bash
   npm install
   ```

## Usage

1. Start the application:
   ```bash
   npm start
   ```

3. Follow the interactive prompts:
- Enter the number of wallets you want to generate
- Select the blockchain network
- View the generated wallets
- Choose to generate more or exit

## Output Format

The generated wallets are saved in the `wallets` directory, organized by network type:

```
wallets/
├── evm/
│   └── evm_wallets.json
└── solana/
    └── solana_wallets.json
```

### EVM Wallet Format
```json
{
  "network": "evm",
  "createdAt": "2024-02-20T12:34:56.789Z",
  "numberOfWallets": 1,
  "wallets": [
    {
      "index": 1,
      "address": "0x...",
      "privateKey": "0x...",
      "mnemonic": "word1 word2 ... word12"
    }
  ]
}
```

### Solana Wallet Format
```json
{
  "network": "solana",
  "createdAt": "2024-02-20T12:34:56.789Z",
  "numberOfWallets": 1,
  "wallets": [
    {
      "index": 1,
      "address": "...",
      "privateKey": "..."
    }
  ]
}
```

## Security

- Private keys and mnemonics are sensitive information. Keep them secure and never share them.
- The generated wallets are saved locally on your machine.
- It's recommended to use this tool on a secure, offline computer.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

This tool is for educational purposes only. Always verify the generated addresses and keep your private keys secure. The author is not responsible for any loss of funds.

---
