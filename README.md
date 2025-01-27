# Sharkbucks

## Introduction

Welcome to Sharkbucks - your gateway to revolutionizing financial inclusion! 🦈💼

Sharkbucks is a cutting-edge auction platform designed to unite investors and SMEs seamlessly. Our platform offers investors easy access to pitches and a plethora of resources, empowering them to bid on loan tenures, interest amounts, and capital, all while competing with other investors. With our finely-tuned Machine Learning model, we ensure that SMEs are matched with investors whose preferences align, optimizing the investment process. For SMEs, Sharkbucks offers unparalleled access to competitive loan offers, facilitating easy access to much-needed funds. Our platform operates on a small platform fee, charged only upon the successful approval of a loan application, ensuring sustainability while providing essential services to both investors and SMEs. Sharkbucks platform also offers a NLP Chatbot feature that serves as a valuable resource for navigating government schemes and exploring investment opportunities, serving as a useful tool for both SMEs and Investors alike.

### Presentation Link : [Drive](https://drive.google.com/file/d/18jro9yVBT8Hoh17EqU1Okyy1JAoUWs75/view?usp=sharing)

### Demo Video Link :  [Drive](https://drive.google.com/file/d/1tGseSuNU1rtm8VCTEkXZg5Bg1J3g_opw/view)

## Features

- **Investor Access**: Investors can easily access pitches and resources to bid on loan tenures, interest amounts, and capital.
- **Machine Learning Model**: Our platform utilizes a finely-tuned ML model to match SMEs with investors whose preferences align, streamlining the investment process.
- **SME Access**: SMEs gain access to competitive loan offers, facilitating easy access to much-needed funds.
- **Sustainable Model**: Sharkbucks operates on a small platform fee, charged only upon the successful approval of a loan application, ensuring sustainability.
- **NLP Chatbot Feature**: The platform offers an NLP Chatbot feature for navigating government schemes and exploring investment opportunities.
- **ZetaChain Integration**: The platform leverages ZetaChain to ensure secure and efficient cross-chain interactions for decentralized crowdfunding.

## Getting Started

To get started with Sharkbucks, follow these steps:

1. **Clone the Repository**: `git clone https://github.com/your-username/sharkbucks.git`
2. **Install Dependencies**: `cd sharkbucks` and `npm install`
3. **Run the Application**: `npm run dev`
4. **Start Blockchain server**: `truffle develop`

## ZetaChain Implementation

Sharkbucks integrates with ZetaChain for cross-chain interactions. Here’s how you can set up and run the ZetaChain integration:

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [Truffle](https://www.trufflesuite.com/truffle)
- [Ganache](https://www.trufflesuite.com/ganache)
- ZetaChain SDK (if available)

### ZetaChain Configuration

1. **Install ZetaChain SDK**: Follow the ZetaChain documentation to install and configure the SDK.

2. **Configure Network**: Add ZetaChain network configuration in your Truffle configuration file (`truffle-config.js`).

```javascript
module.exports = {
  networks: {
    zetachain: {
      provider: () => new HDWalletProvider(mnemonic, "https://zetachain-rpc-url"),
      network_id: 1337,
      gas: 4500000,
      gasPrice: 10000000000,
    },
    // other network configurations
  },
  compilers: {
    solc: {
      version: "0.8.6",
    },
  },
};
```

### Deploying Contracts on ZetaChain

1. **Migrate Contracts**: Use Truffle to deploy your contracts on ZetaChain.

```sh
truffle migrate --network zetachain
```


## Contributors

Sharkbucks was created by Team Nos Code during HackBanglore 2024. For the full list of Contributors check [CONTRIBUTORS](https://github.com/Akash-Singh04/Sharkbucks/graphs/contributors) 

- [Akash Singh](https://github.com/Akash-Singh04)
- [Tarun Kataruka](https://github.com/Tarun-Kataruka)
- [Hemamalini Srinivas](https://github.com/1DS22CS091hemamalini)
- [Abhyuday Hari Prasad](https://github.com/abhyudayhari)

## Contributing

We welcome contributions from the community to enhance Sharkbucks further! To contribute, follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature`)
6. Create a new Pull Request

## License

This project is licensed under the [MIT License](LICENSE).
