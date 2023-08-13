---
title: "Revoke Token Allowances"
description: "Revoke Token Allowances"
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

## BitindiWallet empowers users to manage and revoke token allowances for any DApps they have interacted with in the past. Understanding token allowances and their potential risks can help users better protect their funds while enjoying the convenience of web3 activities.

### Understanding token allowances

A token allowance is a feature of Ethereum and EVMs such as Polygon or Binance Smart Chain that allows DApps to independently access and use funds with specified permissions. These token allowances grant DApps access to a users’s ERC-20 and similar tokens for various types of transactions.

Token swaps offer a good example of how it works:

Swapping token A for token B requires the DApp to withdraw token A from a user’s wallet and send the corresponding amount of token B.

Each token allowance is specific to a particular token, allowing access only to the designated token.

Granting a token allowance streamlines transactions by eliminating repetitive permissions, improving the efficiency of web3 and it’s growing ecosystems.

### Importance of revoking token allowances

Granting token allowances is a standard practice in web3, and is typically not an issue. However, DApps can be susceptible to exploits or hacking attempts, putting funds at risk. Furthermore, unlimited token allowances could enable bad actors to exploit a DApps’s code through a vulnerability and execute unauthorized withdrawals.

Malicious sites may request token approvals in an attempt to steal tokens, imitating legitimate platforms. It is very important to do proper due diligence before granting token allowances, as clicking ‘approve’ could compromise your funds.

### How to revoke allowances in BitindiWallet?

We get it, we know that web3 is constantly evolving and with that comes a growing list of token allowances. BitindiWallet allows users to control token allowances and protect their assets from potential scams. We think it is a good idea to develop a habit of reviewing your token allowances and revoking any that raise concern.

Keep in mind: Just as you paid a gas fee when approving a token allowance, you'll also need to cover gas fees when revoking them through on-chain transactions.

BitindiWallet makes it easy to do directly from your wallet:

- Open Settings by clicking the gear icon in the top right corner of your wallet.

![Revoke_Allowance_1_40c05bbd09](https://github.com/bitindi/docs/assets/119077822/604a73cc-1556-40e6-9be7-6003ca5798bb)

- Click Account.

![Revoke_Allowance_2_bbfeaac033](https://github.com/bitindi/docs/assets/119077822/2bda24b1-69cb-46b9-8b67-1caf83645ca7)

- Click Token Allowances.

![Revoke_Allowance_3_ccacb2205f](https://github.com/bitindi/docs/assets/119077822/8e89827f-c336-4cee-a851-0cd94ebba12c)

- Search for the allowance you want to revoke by token (e.g., USDT, DAI, USDC) or spender (e.g., 1Inch, LiFi, Uniswap).
- Optionally, group allowances by spender or token to revoke a specific group of allowances.
- Click Revoke next to the desired allowance.
- Confirm the transaction to reset the token allowance to zero (0).

![Revoke_Allowance_4_56fb8af484](https://github.com/bitindi/docs/assets/119077822/3dbe570d-c5fd-43ff-bb63-7e4bce7b7a5f)

For a more efficient approach, click Revoke All on the token allowances screen to revoke all token allowances at once. This feature allows you to consecutively remove all allowances in your wallet without revisiting the Token Allowance page for each action.

Alternatively, you can access token allowances by clicking any asset in your Assets list and clicking the Allowances tab, then Manage Allowances.



