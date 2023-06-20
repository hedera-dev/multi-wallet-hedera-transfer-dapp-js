Transfer Hedera tokens with ease using this DApp built on the Create React App Hedera DApp template. It leverages Material UI and JavaScript, providing support for HashPack, Blade, and MetaMask wallets.

## Prerequisites

### Hedera Testnet account

Don't have one? Create one by going to [portal.hedera.com](https://portal.hedera.com/register). This testnet account will recieve 10,000 test HBAR every 24 hours!

### Hashpack Wallet
* Install the [Hashpack extension](https://chrome.google.com/webstore/detail/hashpack/gjagmgiddbbciopjhllkdnddhcglnemk).  
* Import a Hedera ED25519 testnet account into Hashpack.

### Blade Wallet
* Install the [Blade extension](https://chrome.google.com/webstore/detail/blade-%E2%80%93-hedera-web3-digit/abogmiocnneedmmepnohnhlijcjpcifd).  
* Import a Hedera ED25519 testnet account into Blade.

### Metamask Wallet
* Install the [MetaMask extension](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn).  

#### How to activate your account on Hedera Testnet

* Activate it by transferring any amount of test HBAR to your EVM address

-----

## How to use

### Locally
1. Fork the repository
2. Clone your forked version
3. Execute ```npm i```
4. Execute ```npm run start``` to start the project

> Blade requires the use of HTTPS in order to pair wallets. An `.env` file exists in your root directory with `HTTPS=true` in order to connect to blade.

----

## JSON RPC Relay Endpoint Alternatives
This DApp utilizes [Hashio](https://swirldslabs.com/hashio/) to connect to Hedera Testnet over RPC.
There are three options available to establish a connection to Hedera Networks:
* Hashio
* Arkhia
* Hedera JSON RPC Relay

Follow the guide [how to connect to Hedera Networks over RPC](https://docs.hedera.com/hedera/tutorials/more-tutorials/json-rpc-connections) to connect using Arkhia or a local version of the Hedera JSON RPC Relay.

## Resources
* [The Hedera DApp CRA Template](https://github.com/hedera-dev/cra-hedera-dapp-template)
* Need to quickly create Hedera Testnet accounts to act as Sender/Receiver? Check out [Create Hedera Accounts with Tokens Helper](https://github.com/hedera-dev/hedera-create-account-and-token-helper)
* [Hashscan](https://hashscan.io/testnet/dashboard) network explorer
