# Hedera DApp with MetaMask, HashPack, and Blade Integration
Transfer Hedera tokens with ease using this DApp built on the Create React App Hedera DApp template. It leverages Material UI and JavaScript, providing support for HashPack, Blade, and MetaMask wallets.

## Tutorial
This repo is intended to be used alongside the tutorial:
[How to use my example project](https://docs.hedera.com/tutorials/my-example-project)

To follow along, start with the `main` branch,
which is the default branch of this repo.
This gives you the initial state from which you can follow along
with the steps as described in the tutorial.

```shell
git clone git+ssh://git@github.com/hedera-dev/cra-hedera-dapp-template.git
```

To skip ahead to the final state, use the `completed` branch.
This gives you the final state with which you can compare your implementation
to the completed steps of the tutorial.

```shell
git fetch origin completed:complete
git checkout completed
```
## Completed Branch Usage

1. Execute ```npm i```
2. Execute ```npm run start``` to start the project

> Blade requires the use of HTTPS in order to pair wallets. An `.env` file exists in your root directory with `HTTPS=true` in order to connect to blade.

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

## Configuration
This project uses a configuration file located `src/config/networks.ts`.

```JavaScript
export const networkConfig = {
  testnet: {
    network: "testnet",
    jsonRpcUrl: "https://testnet.hashio.io/api", // check out the readme for alternative RPC Relay urls
    mirrorNodeUrl: "https://testnet.mirrornode.hedera.com",
    chainId: "0x128",
  }
}
```

---

## JSON RPC Relay Endpoint Alternatives
This DApp utilizes [Hashio](https://swirldslabs.com/hashio/) to connect to Hedera Testnet over RPC.
There are three options available to establish a connection to Hedera Networks:
* Hashio
* Arkhia
* Hedera JSON RPC Relay

Follow the guide [how to connect to Hedera Networks over RPC](https://docs.hedera.com/hedera/tutorials/more-tutorials/json-rpc-connections) to connect using Arkhia or a local version of the Hedera JSON RPC Relay.

## Links
* [The Hedera DApp CRA Template](https://github.com/hedera-dev/cra-hedera-dapp-template)
* Need to quickly create Hedera Testnet accounts to act as Sender/Receiver? Check out [Create Hedera Accounts with Tokens Helper](https://github.com/hedera-dev/hedera-create-account-and-token-helper)
* [Hashscan](https://hashscan.io/testnet/dashboard) network explorer
