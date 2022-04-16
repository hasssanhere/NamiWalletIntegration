# Nami Wallet examples
## About Nami Wallet
Nami Wallet is a browser-based wallet extension to interact with the Cardano blockchain. It's an open-source project and built by Berry Pool.

You can download the wallet for different browsers here ([https://namiwallet.io](https://namiwallet.io/))

If you find this repository useful and want to support us, you can donate ADA to this wallet ```addr1qysjrwqv6uyu7gtwtzvhjceauj8axmrhssqf3cvxangadqzt5f4xjh3za5jug5rw9uykv2klc5c66uzahu65vajvfscshgt2vq```. 
## Setup
To run the application locally these installation steps:
```
// Install packages for application
npm install

// Install the module with cardano serialization lib
cd src/nami-js
npm install

// Return to workspace
cd ../..
```
To run the application start the node process with
```
npm run start
```
Run our example app to try out the functionalities of our package.

Before you can use the NamiWalletApi you have to create an account to get a blockfrost api key https://blockfrost.io/.
Create a ```./config.js``` file and add your API key information.
```js
const blockfrostApiKey = {
    0: "rbkrp5hOr3khPAWNo3x47t6CP7qKFyA5", // testnet
    1: "mainnetfqH0CVlBesnsj5IKhgIYCn231KzqUOyk" // mainnet
}

export default blockfrostApiKey;
```

