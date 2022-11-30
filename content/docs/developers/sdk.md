---
title: "On-chain interaction"
description: "Bitindi is compatible with Ethereum's ecosystem，support all Ethereum's RPC API and SDK。"
lead: "Bitindi is compatible with Ethereum's ecosystem，support all Ethereum's RPC API and SDK."
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

### RPC

RPC Method List Example:
```
curl -s -H 'content-type:application/json' -d '{"jsonrpc":"2.0","method":"web3_clientVersion","params":[],"id":67}' http://localhost:8545
```

## SDK

Use `Ethereum` SDK library such as `web3j`,`web3js`, etc for development.

## Get chain info

```
const Web3 = require('web3')

async function getChainId() {
    const web3 = new Web3('https://rpc-mainnet.bitindi.io')
    let chainId = await web3.eth.getChainId()
    console.log(`chain id: ${chainId}`)
    return chainId
}
```
## Generate account

```
const Web3Accounts = require('web3-eth-accounts')

let account = new Web3Accounts().create()
//do not do this on prd env
console.log(`account generated. address: ${account.address}, private key: ${account.privateKey}`)
```

## Build transaction
```
const Web3 = require('web3')

async function transfer(fromAccount, to, value){
    const web3 = new Web3('https://rpc-mainnet.bitindi.io')
    let chainId = await web3.eth.getChainId()
    let nonce = await web3.eth.getTransactionCount(fromAccount.address)
    let gasPrice = await web3.eth.getGasPrice()

    let unsigned = {
        from: fromAccount.address,
        to,
        value: web3.utils.numberToHex(web3.utils.toWei(value, 'ether')),
        gasPrice,
        nonce,
        chainId,
    }

    unsigned.gas = await web3.eth.estimateGas(unsigned)

    let signed = await fromAccount.signTransaction(unsigned)
    return signed
}
```