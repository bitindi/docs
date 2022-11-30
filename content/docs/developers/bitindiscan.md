---
title: "Bitindi Scan"
description: "Bitindi Scan is more than just a block explorer. It contains useful resources that developers can leverage for their dapps, such as the PostgreSQL database layer, GraphQL server and smart contract APIs."
lead: "Bitindi Scan is more than just a block explorer. It contains useful resources that developers can leverage for their dapps, such as the PostgreSQL database layer, GraphQL server and smart contract APIs."
date: 2022-10-13T15:21:01+02:00
lastmod: 2022-10-13T15:21:01+02:00
draft: false
images: []
menu:
  docs:
    parent: "developers"
weight: 270
toc: true
---

## Bitindi chain data
Most apps require a fast and efficient data source for things that are not easily available over raw
blockchain RPC, for example:
 - balances of all tokens that a user has
 - list of token holders for a particular coin
 - history of token trades on a DEX
 - history of user's interaction with a smart contract


Bitindi Scan offers 3 solutions for various use cases:
 - GraphQL server for web apps
 - PostgreSQL database for advanced apps and data analysis
 - HTTP API for developers

### The Graph
Bitindi Scan comes with a public GraphQL service, also known as "The Graph".

It is available for both mainnet and testnet, on `/graphql`:
```
Mainnet: https://bitindiscan.com/graphiql
Testnet: https://testnet.bitindiscan.com/graphiql