---
title: "Net Worth"
description: "Net Worth"
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

## You can find a quick snapshot of your cumulative net worth directly on the BitindiWallet home screen. This value is specific to the account, and chain that is currently selected.

![Net_Worth_13705e4caf](https://github.com/bitindi/docs/assets/119077822/94b78fc2-fae2-45d7-8a78-07fd0820013f)

### How does it work?
Net Worth is simply the sum of all assets in your wallet denominated by the currency selected in your wallet. The value will be displayed in USD by default, with the option to change the currency by navigating to *Preferences > Locale Configuration*.

### How is my net worth calculated?

Based on the holdings from your Assets list, BitindiWallet fetches token prices from CoinGecko, before calculating the sum of all your assets to get your total net worth.

Keep in mind that BitindiWallet only considers the tokens currently visible on your Assets list for the net worth calculation. The net worth displayed on BitindiWallet may differ from the one shown on a block explorer due to exclusions on your Asset list.

### Troubleshooting

If you believe the net worth being displayed is inaccurate, here are some easy questions to troubleshoot the problem:

- Do all your tokens have an associated fiat value in the Assets list? If not, try resetting the wallet or switching back and forth from another network to trigger a reload.
- Do all your assets appear in your Assets list? Make sure all your token holdings appear in your Assets list. If not, you can add it by clicking “+ Add Token” at the bottom of the list.

### Remember, this feature shows an approximate value. The actual value in fiat might differ after swaps and bridges.

### Are my NFTs counted in my Net Worth?
No. Your NFTs are not counted in Net Worth (yet). You can check for a more detailed breakdown of your net worth with a service like [https://zapper.xyz/](https://zapper.xyz/)
