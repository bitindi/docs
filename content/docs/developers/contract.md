---
title: "Contract"
description: "Bitindi uses EVM for contract execution.See Solidity for detail."
lead: "Bitindi uses EVM for contract execution.See Solidity for detail."
date: 2022-10-13T15:21:01+02:00
lastmod: 2022-10-13T15:21:01+02:00
draft: false
images: []
menu:
  docs:
    parent: "developers"
weight: 240
toc: true
---

### Remix

Remix IDE is an open source web and desktop application. It fosters a fast development cycle and has a rich set of plugins with intuitive GUIs. Remix is used for the entire journey of contract development as well as being a playground for learning and teaching contract development.

![](https://github.com/bitindi/bitindi/blob/main/assets/images/remix1.jpg?raw=true)

Create new file in file explorer. Edit contract info at right side.

![](https://github.com/bitindi/bitindi/blob/main/assets/images/remix2.jpg?raw=true)

Compile contract

- Click compiler button, switch UI
- Select contract you want to compile
- Set compile flags
- Clieck compile button

![](https://github.com/bitindi/bitindi/blob/main/assets/images/remix3.jpg?raw=true)

Deploy contract to blockchain via wallet such as `MetaMask`.

- Set network info in `Metamask`.

![](https://github.com/bitindi/bitindi/blob/main/assets/images/meta.png?raw=true)


- Back to Remix.
- Swich environment
- Select contract
- click deploy button

![](https://github.com/bitindi/bitindi/blob/main/assets/images/remix4.jpg?raw=true)

The contract can be deployed on the chain through MetaMask

## Truffle
Use truffle to compile and deploy contract.

- Install Node.js See [Installing Node.js](https://nodejs.org/en/download/package-manager/) for detail.

- Install truffle

```
npm install -g truffle
```
Run `truffle version` after installation finished. If the command line displays a message like below, installation is successful.

```
Truffle v5.1.36 (core: 5.1.36)
Solidity v0.5.16 (solc-js)
Node v10.22.1
Web3.js v1.2.1
```

- Create project
First,create folder for project.

```
mkdir Example
cd Example
```

Then, init project via truffle

```
truffle init
```

After initialization is complete, the following file structure is generated within the project.

```
|-- contracts         //folder for contracts
|-- migrations        //folder for deployment scripts
|-- test              //folder for test scripts
|-- truffle-config.js //truffle config file
```
- Config truffle info

```
const HDWalletProvider = require('@truffle/hdwallet-provider');

const fs = require('fs');
const mnemonic = fs.readFileSync(".secret").toString().trim();

module.exports = {
  networks: {
    testnet: {
      provider: () => new HDWalletProvider(mnemonic, 'https://rpc-testnet.bitindi.org'),
      network_id: 34
    },
    mainnet: {
      provider: () => new HDWalletProvider(mnemonic, 'https://rpc-mainnet.bitindi.org'),
      network_id: 24
    }
  },

  // Set default mocha options here, use special reporters etc.
  mocha: {
    // timeout: 100000
  },

  // Configure your compilers
  compilers: {
    solc: {
      // version: "0.5.1",    // Fetch exact version from solc-bin (default: truffle's version)
      // docker: true,        // Use "0.5.1" you've installed locally with docker (default: false)
      // settings: {          // See the solidity docs for advice about optimization and evmVersion
      //  optimizer: {
      //    enabled: false,
      //    runs: 200
      //  },
      //  evmVersion: "byzantium"
      // }
    },
  },
};
```

- Create contract Put custom contracts into folder `contracts` and modify deployment script in folder `migrations`.

- Deploy contract

Run the deployment command.

```
truffle migrate --network testnet
```

The output as below.

```
2_example_migration.js
======================

   Deploying 'ExampleToken'
   ------------------------
   > transaction hash:    0x91e50594a63bc6f4c299f3f445868571678be306b835bddce6dff5c7a5ddf9dc
   > Blocks: 2            Seconds: 4
   > contract address:    0x54D2049715FC8De1361D7350de90eb05F0f6CA84
   > block number:        375304
   > block timestamp:     1608016637
   > account:             0x03D32B774295D740ffEe43b20fcC0a53acC576e6
   > balance:             878.909609236165318643
   > gas used:            1056044 (0x101d2c)
   > gas price:           20 gwei
   > value sent:          0 BNI
   > total cost:          0.00112088 BNI


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00112088 BNI


Summary
=======
> Total deployments:   1
> Final cost:          0.00112088 BNI
```

Finally, the contract deployment is complete.
