# MetaDex

A decentralized exchange protocol built on Uniswap v4, implementing custom hooks for enhanced trading features and fee distribution.

## Overview

MetaDex extends Uniswap v4's functionality by implementing custom hooks that enable:
- Token locking and voting mechanisms
- Fee collection and distribution
- LP provider emissions
- Custom swap logic

## Architecture

- **Token Locking & Voting**: Users can lock tokens to participate in governance and earn fees
- **Uniswap v4 Integration**: Custom hooks capture swap fees in real-time
- **Fee Distribution**: Automated distribution of collected fees to token lockers
- **LP Emissions**: Additional rewards for liquidity providers

## Prerequisites

- [Foundry](https://book.getfoundry.sh/getting-started/installation.html)
- [Git](https://git-scm.com/downloads)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/MetaDex.git
cd MetaDex
```

2. Install dependencies:
```bash
forge install
```

## Development

### Build

```bash
forge build
```

### Test

```bash
forge test
```

### Deploy

```bash
forge script script/Deploy.s.sol:Deploy --rpc-url <your_rpc_url> --broadcast
```

## Project Structure

```
├── src/
│   └── MetaDexHook.sol       # Main hook implementation
├── test/
│   └── MetaDexHook.t.sol     # Test suite
├── script/
│   └── Deploy.s.sol          # Deployment scripts
└── lib/                      # Dependencies
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Uniswap v4](https://github.com/Uniswap/v4-core)
- [Foundry](https://github.com/foundry-rs/foundry)
