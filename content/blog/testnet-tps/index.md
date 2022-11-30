---
title: "Bitindi testnet stress test"
description: "Bitindi chain stress test yields ~ 2500 TPS (transactions per second)."
lead: ""
date: 2022-11-09T00:00:00+02:00
lastmod: 2022-11-09T00:00:00+02:00
draft: false
weight: 50
images: []
contributors: ["Bitindi Developers"]
---

We have ran multiple stress tests on Bitindi testnet to benchmark Bitindi chain's performance.

### Methodology
Bitindi testnet is currently running the same runtime and configuration as Bitindi mainnet, therefore
these results are also indicative of mainnet performance. The transactions were broadcasted through
a regular Bitindi node, without any optimizations.

We have prepared and broadcasted two types of transactions to test for both on-chain and EVM throughput.

For the EVM throughput, ERC-20 token transfers were chosen, as they are the most common transaction
type on Ethereum.

### Results
The **EVM token transfer test yielded 2500 TPS** (transactions per second), while a slighly more complex
on-chain transfers yielded 2500 TPS.

The current throughput seems to be around 200x higher than Ethereum, thanks to the more efficient
BPoS consensus and modern blockchain architecture.

### Future improvements
Bitindi chain can scale its throughput further by sharding. Currently, the allowance is 2s out of 3s block time to ensure everyone
can run a full node from anywhere in the world, using only modest hardware ($10/mo VPS should be
sufficient).

