---
title: "Quick start"
description: "Get quickly up and running with Bitindi chain"
lead: ""
date: 2022-11-16T13:59:39+01:00
lastmod: 2022-11-16T13:59:39+01:00
draft: false
images: []
menu:
  docs:
    parent: "developers"
weight: 200
toc: true
---

In this guide we will deploy a simple smart contract onto Bitindi chain.


### (Optional) Setting up a development node

To set up your local development or RPC node, check out the [Bitindi node guide](/docs/developers/nodes/).


## New to Solidity?
Solidity is a programming language for writing DeFi applications. The Solidity programs are compiled
and uploaded to Bitindi chain, where they run in a completely decentralized fashion.

Here are some great resources for learning Solidity:
 - The [official Solidity docs](https://docs.soliditylang.org)
 - Solidity [tutorial](https://www.tutorialspoint.com/solidity/index.htm) for programmers

## Smart Contracts on Bitindi vs Ethereum

{{< alert icon="💡" text="Bitindi chain is based on Ethereum Go. Bitindi supports all Ethereum smart contracts on Bitindi Chain. And, many tools of Ethereum such as Metamask and web3 are compatible." >}}

The Bitindi chain smart contracts are written in [Solidity](https://docs.soliditylang.org/en/latest/).
Any existing Ethereum smart contracts written in Solidity 0.6 or greater will work on Bitindi chain
without a need for modifications.

## Deploy your first BIP-20 Token

We are going to pick a simple ERC-20 contract for our demo, but feel free to try out other examples as well.

In this guide we are using [Hardhat](https://hardhat.org/), which is
suitable for more experienced developers. If you would like to deploy your contract via an easy to
use web IDE, try [Remix](https://remix.ethereum.org/).

### Clone the examples repo
{{< btn-copy text="git clone https://github.com/bitindi/hardhat-examples" >}}
```bash
git clone https://github.com/bitindi/hardhat-examples
```

### Install the dependencies
{{< btn-copy text="yarn" >}}
```bash
yarn
```

### Run the deployment script

{{< btn-copy text="npx hardhat run scripts/erc20/deploy.js" >}}
```bash
npx hardhat run scripts/erc20/deploy.js
```

## Interact with the BIP-20 to send tokens

We can call functions on our smart contract through the Hardhat interface:



## Next steps

Congratulations. You now have a running development node with the first smart contract. You and now are ready to start building your first DeFi app.

### Deploy on testnet
Deploying on testnet is similar to development, however there are 2 things we need.

1.) Run a testnet node or use the public [testnet RPC](/docs/developers/networks/#testnet-info-sheet).

2.) Create an [account](/docs/developers/accounts/) and obtain testnet BNI tokens from the faucet.

To get 1000 BNI testnet tokens simply type visit faucet [Faucet](https://faucet.bitindiorg).

### Deploy on mainnet
Deploying on mainnet is similar to development, however there are 2 things we need.

1.) Run a mainnet node or use the public [mainnet RPC](/docs/developers/networks/#mainnet-info-sheet).

2.) Create an [account](/docs/developers/accounts/) and obtain Bitindi chain native BNI tokens from
the bridge, swap or exchange.

### Verify the contract on Bitindi Scan
Once you have deployed your smart contract on Bitindi Chain mainnet (or testnet), you will want to
verify it on Bitindi Scan, so that other developers can access its source code and ABI.

Verify your deployed contract on: [Mainnet](https://bitindiscan.com/accounts) or [Testnet](https://testnet.bitindiscan.com/accounts)

{{< alert icon="💡" text="Remix and Hardhat support automatic contract verification. You can skip this step if you use either of those tools." >}}