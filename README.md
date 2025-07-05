# ChatterPay Subgraph for Deposits 📈

![ChatterPay](https://img.shields.io/badge/ChatterPay-Subgraph-4A90E2?style=for-the-badge&logo=ethereum)

Welcome to the **ChatterPay-Subgraph-Deposits** repository! This project tracks deposits made from non-Chatters to ChatterPay accounts. With the rise of decentralized finance (DeFi) and account abstraction, monitoring these transactions is essential for both users and developers.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Overview

ChatterPay is a platform designed to facilitate seamless transactions in the crypto space. This subgraph specifically focuses on tracking deposits made by non-Chatters to ChatterPay accounts. By utilizing The Graph protocol, we can efficiently index and query blockchain data.

## Features

- **Real-time Tracking**: Monitor deposits as they happen.
- **User-Friendly Queries**: Access data easily with GraphQL.
- **Decentralized Architecture**: Built on a secure and transparent network.
- **Support for Multiple Tokens**: Works with USDT, WBTC, WETH, and more.

## Technologies Used

- **The Graph**: For indexing and querying blockchain data.
- **TypeScript**: For building a robust and maintainable codebase.
- **Scroll Network**: A layer 2 solution for Ethereum.
- **Account Abstraction**: Enhances user experience by simplifying wallet interactions.

## Getting Started

To get started with the ChatterPay Subgraph, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Stej13Dd/ChatterPay-Subgraph-Deposits.git
   cd ChatterPay-Subgraph-Deposits
   ```

2. **Install Dependencies**:
   Make sure you have Node.js installed. Then run:
   ```bash
   npm install
   ```

3. **Deploy the Subgraph**:
   You can deploy the subgraph using the following command:
   ```bash
   graph deploy <YOUR_SUBGRAPH_NAME>
   ```

4. **Run the Subgraph**:
   To run the subgraph locally, use:
   ```bash
   graph codegen
   graph build
   graph deploy --local
   ```

## Usage

Once the subgraph is running, you can query it using GraphQL. Here are some example queries:

### Fetch All Deposits

```graphql
{
  deposits {
    id
    amount
    token
    timestamp
  }
}
```

### Fetch Deposits by User

```graphql
{
  deposits(where: { user: "0x1234567890abcdef" }) {
    id
    amount
    token
    timestamp
  }
}
```

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or suggestions, please reach out to the project maintainers:

- **Stej13Dd**: [GitHub Profile](https://github.com/Stej13Dd)

## Releases

To download and execute the latest release, visit [Releases](https://github.com/Stej13Dd/ChatterPay-Subgraph-Deposits/releases). Check the releases section for updates and new features.

![Releases](https://img.shields.io/badge/Releases-Click_here-FF5722?style=for-the-badge)

## Conclusion

Thank you for checking out the ChatterPay Subgraph for Deposits. We hope this project helps you understand and track deposits in the ChatterPay ecosystem. Happy coding!