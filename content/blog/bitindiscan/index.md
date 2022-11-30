---
title: "Bitindi Scan is live"
description: "Bitindi Scan is live. Bitindi Scan is the main Bitindi chain block explorer."
lead: ""
date: 2022-11-28T07:45:48+02:00
lastmod: 2022-11-28T07:45:48+02:00
draft: false
weight: 50
images: []
contributors: ["Bitindi Developers"]
---

[Bitindiscan](https://bitindiscan.com) is the most advanced, fully open-source block explorer. It was built from
the ground up for Bitindi chain.

## Bitindi UI Redesign
Bitindi scan has a new look. It is the first Bitindi project utilizing components from the upcoming [Bitindi  UI kit](/docs/developers/ui_kit/).

![](https://github.com/bitindi/bitindi/blob/main/assets/images/redesign.png?raw=true)

## BIP-20 Token Tracker
Bitindi scan will now automatically label and track smart contracts that satisfy BIP-20 contract interface.
This gives users the full transparency into token holdings and token movements on chain.

## Improved smart contract support
Smart contracts now have a full source viewer and improved verification API. The verification APIs
are also integrated into [Hardhat](https://hardhat.org/) and [Remix](https://remix.ethereum.org/).

## The Graph
Bitindi scan's choice of database backend - Postgres - will certainly delight many software engineers.
However we have received a lot of requests for "The graph". Fortunately, Bitindi Scan also ships with
Hasura GraphQL server which makes it easy for web developers to connect with Bitindi chain
data warehouse for faster and more powerful frontend applications.

Check out the [Bitindi scan documentation](/docs/developers/bitindiscan/) to learn how to access the graph
and other features.

## Bitindi scan APIs
Bitindi scan also ships with multiple API endpoints that are useful for quickly implementing wallet
enhancements and other features:
 - An API for listing user's tokens and balances
 - An API for historic trading data on Bitindi swap DEX
 - An API for programmatically verifying smart contracts source code
 - An API for retreiving verified smart contract's source and ABI


