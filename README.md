# BlockGrid

A Stacks blockchain smart contract project built with Clarity, designed for decentralized grid-based applications on the Stacks network.

## 🚀 Overview

BlockGrid is a smart contract project that leverages the Stacks blockchain and Clarity smart contract language. This project provides a foundation for building decentralized applications with grid-based functionality, utilizing the security and programmability of the Stacks ecosystem.

## 🛠 Technology Stack

- **Blockchain**: Stacks (STX)
- **Smart Contract Language**: Clarity
- **Development Framework**: Clarinet
- **Testing Framework**: Vitest with Clarinet SDK
- **Language**: TypeScript for tests
- **Package Manager**: npm

## 📁 Project Structure

```
blockgrid/
├── contracts/
│   └── blockgrid.clar          # Main Clarity smart contract
├── tests/
│   └── blockgrid.test.ts       # TypeScript test files
├── settings/
│   ├── Devnet.toml            # Development network configuration
│   ├── Testnet.toml           # Testnet configuration
│   └── Mainnet.toml           # Mainnet configuration
├── Clarinet.toml              # Clarinet project configuration
├── package.json               # Node.js dependencies and scripts
├── tsconfig.json              # TypeScript configuration
├── vitest.config.js           # Vitest testing configuration
└── README.md                  # Project documentation
```

## 🔧 Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v16 or higher)
- [Clarinet](https://github.com/hirosystems/clarinet) - Stacks development tool
- [Git](https://git-scm.com/)

### Installing Clarinet

```bash
# macOS (using Homebrew)
brew install clarinet

# Windows (using Chocolatey)
choco install clarinet

# Linux (using curl)
curl -L https://github.com/hirosystems/clarinet/releases/latest/download/clarinet-linux-x64.tar.gz | tar xz
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/ojerindeolamide/BlockGrid.git
cd BlockGrid
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Run Tests

```bash
# Run all tests
npm test

# Run tests with coverage and cost reports
npm run test:report

# Watch mode for continuous testing
npm run test:watch
```

## 🧪 Testing

The project uses Vitest with the Clarinet SDK for comprehensive testing:

- **Unit Tests**: Located in `tests/blockgrid.test.ts`
- **Simnet Integration**: Tests run against a simulated Stacks network
- **Coverage Reports**: Generate detailed coverage and cost analysis
- **Continuous Testing**: Watch mode for development

### Test Commands

```bash
# Basic test run
npm test

# Test with coverage and cost analysis
npm run test:report

# Continuous testing (watches for file changes)
npm run test:watch
```

## 🌐 Network Configuration

### Development Network (Devnet)

The project includes a comprehensive devnet configuration with:
- Pre-configured wallet accounts with STX and sBTC balances
- Local blockchain simulation
- Multiple test accounts for complex scenarios

### Testnet Deployment

To deploy to Stacks testnet:

1. Update `settings/Testnet.toml` with your testnet mnemonic
2. Use Clarinet deployment commands

### Mainnet Deployment

For mainnet deployment:

1. Update `settings/Mainnet.toml` with your mainnet mnemonic
2. Ensure thorough testing on testnet first
3. Use appropriate deployment fee rates

## 📝 Smart Contract Development

### Clarity Contract Structure

The main contract (`contracts/blockgrid.clar`) follows Clarity best practices:

```clarity
;; Contract sections:
;; - Traits: Interface definitions
;; - Token definitions: Fungible/Non-fungible tokens
;; - Constants: Immutable values
;; - Data vars: Mutable contract state
;; - Data maps: Key-value storage
;; - Public functions: External callable functions
;; - Read-only functions: View functions
;; - Private functions: Internal helper functions
```

### Development Workflow

1. **Write Clarity Code**: Develop smart contract logic in `contracts/blockgrid.clar`
2. **Write Tests**: Create comprehensive tests in `tests/blockgrid.test.ts`
3. **Run Tests**: Validate functionality with `npm test`
4. **Deploy**: Use Clarinet for deployment to various networks

## 🔍 Key Features

- **Modular Architecture**: Clean separation of concerns
- **Comprehensive Testing**: Full test coverage with cost analysis
- **Multi-Network Support**: Devnet, testnet, and mainnet configurations
- **Type Safety**: TypeScript integration for robust development
- **Continuous Integration**: Automated testing and validation

## 📚 Resources

- [Stacks Documentation](https://docs.stacks.co/)
- [Clarity Language Reference](https://docs.stacks.co/clarity/)
- [Clarinet Documentation](https://docs.hiro.so/clarinet/)
- [Stacks.js SDK](https://github.com/hirosystems/stacks.js)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **ojerindeolamide** - *Initial work* - [GitHub](https://github.com/ojerindeolamide)

## 🙏 Acknowledgments

- Stacks Foundation for the blockchain infrastructure
- Hiro Systems for development tools and documentation
- The Clarity community for best practices and examples

---

**Note**: This project is in active development. Please refer to the issues and project board for current development status and planned features.
