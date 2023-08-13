---
title: "Add a Network or Custom RPC"
description: "Add a Network or Custom RPC"
lead: ""
date: 2022-10-06T08:48:57+00:00
lastmod: 2022-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "wallet"
weight: 120
toc: true
---

## As the blockchain and web3 ecosystem continues to grow, numerous EVM-compatible networks are emerging. Adding these custom networks to BitindiWallet is easy and essential to be able to interact with your favorite decentralized applications (dApps) and decentralized exchanges (DEXes).

*EVM stands for Ethereum Virtual Machine, which simply means that these networks use similar technology as Ethereum. These networks are supported by BitindiWallet by default. Networks that are built on other technologies are not supported (Bitcoin, Solana eco, Atom eco, Move eco…)*

### What is an RPC?
RPC, or Remote Procedure Call, is a set of protocols that enable BitindiWallet to interact and communicate with a blockchain. It is essential for checking account balances, sending transactions, and interacting with dApps.

When you add a custom network to BitindiWallet, you provide the RPC information necessary for the wallet to establish a connection with a specific network. Adding a custom RPC will allow you to manage the assets for that specific blockchain.

*Keep in mind that adding a network on one device does not automatically add it to another device, even if accessing the same account. If you uninstall the BitindiWallet extension, you will need to re-add custom networks.*

### Add a network to BitindiWallet

To add a custom network, follow these steps:

- From your BitindiWallet dashboard click the gear icon in the top-right corner.

![260317698-b6a1ffcf-781d-4c47-925c-11e4cf656c4e](https://github.com/bitindi/docs/assets/119077822/88c281e5-1dee-418b-af51-7d11d2a1bacf)


- Select Networks.

![Add_Custom_RPC_2_7378adab48](https://github.com/bitindi/docs/assets/119077822/33c96048-528d-47cc-b457-3768ad6e241d)

- Click + Add New Network.

![Add_Custom_RPC_3_3defd88780](https://github.com/bitindi/docs/assets/119077822/d247a750-cf1d-4c71-944e-d6402578c162)

- Enter the network’s Chain ID or Chain Name. (To search for a testnet or networks supported by default, modify your search filter by clicking the menu icon in the top-right corner.)

![Add_Custom_RPC_4_4d59f1f0a1](https://github.com/bitindi/docs/assets/119077822/b1cd1b48-2ea8-4c3c-b863-6ff4511afa71)

If your search yields no results, either you entered the Chain ID or Chain Name incorrectly or the network you are trying to add is not recognized and requires manually adding it to BitindiWallet.

### Use Chainlist to add a custom network

[Chainlist](https://chainlist.org/) is a great resource that provides a list of EVM-compatible networks, which are Ethereum-like blockchains. It simplifies adding custom networks to BitindiWallet, enabling users to connect and interact with various blockchain networks with the click of a button.

We highly recommend exploring the list of networks available on Chainlist, especially for beginners before getting into manually adding a network as the process does not require technical detail like RPC URL or Chain ID.

### Adding a network manually

To add a network manually you will need to have the details for the network and then click click “add it manually”

- Enter the Network Name, RPC URL, Chain ID, and Currency Symbol.
 
- You can also enter a Block Explorer URL if the network has a blockchain explorer.

![Add_Custom_RPC_5_e4856b981b](https://github.com/bitindi/docs/assets/119077822/9bacb0d8-af7a-4656-82da-3b122d93a8ec)

- Click “Save”

![Add_Custom_RPC_7_312de93307](https://github.com/bitindi/docs/assets/119077822/dc0566c4-49c7-4810-beed-8449f37098bc)

### Edit network details

There may be instances where you need to edit network details.

*Editing network details is an advanced feature. If you are not confident about the changes you are making, avoid modifying network details.*

- Ensure that you are NOT currently connected to the network you want to edit. You can switch to any other network.
- Navigate to “Networks” in the settings, select the pencil next to the network that you want to edit.
- Click “Save” when finished.

### Risks of adding unknown networks

Adding custom networks comes with inherent risks, as not all networks can be trusted. Follow these best practices when adding custom networks:

- Due diligence: BitindiWallet does not verify non-recognized networks, therefore ensure that you trust the network before adding it to your wallet.
- Use established bridges or portals: When bridging tokens (moving them from one network to another), ensure you trust the network operator and the receiving address. Sending crypto assets directly from one network or chain to another may result in permanent, irreversible asset loss.
- Verify custom network information: Always double-check the custom network information before adding it to BitindiWallet.

### Reorder your networks

In the Networks menu, you can easily reorder the networks by dragging and dropping them in position. This order will be reflected in the network drop-down on home.








