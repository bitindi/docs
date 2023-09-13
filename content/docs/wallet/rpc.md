---
title: "Protect RPCs"
description: "Front-running protection for transactions on the Ethereum, BSC and Polygon Network."
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
## Public RPCs for Ethereum, BSC, and Polygon

Users can immediately take advantage of bitindi's frontrunning protection/prevention features by routing their transactions through bitindi’s RPC inside their wallets. bitindi currently has the following RPCs available for users:

|  Network Name   | Blockchain  | Chain ID    | Region  | RPC URL  |
| ---------------  | -------------  |----------   | --------- | ----------- |
| ETH Protect   | Ethereum  |1  | Multi | [https://ethpro.bitindi.org](https://ethpro.bitindi.org) |
| ETH Gas Protect  | Ethereum  |1  | Multi | [https://eth.bitindi.org](https://eth.bitindi.org) |
| BSC Protect   | BSC  |1  | Multi | [https://bsc.bitindi.org](https://bsc.bitindi.org) |
| Polygon Protect  | Polygon  | 137  | Multi | [https://polygon.bitindi.org](https://bsc.bitindi.org) |


# ETH Protect RPC

ETH Protect provides reliable and free front-running protection for Metamask and Bitindi Wallet transactions on the Ethereum Mainnet network.
ETH Protect securely sends your transaction directly to block proposers using our high-performance global network. This keeps transactions hidden from front-running and sandwich bots until after the transaction has been mined and the window of opportunity for an attack has passed.
Setup custom ETH Protect RPC in Metamask
1. Open Metamask and click on "Settings"
2. Click on "Networks", and then click on "Add Network" on the Networks menu.
   
![image](https://github.com/bitindi/docs/assets/119077822/430da26f-7f1a-4162-a21d-f9381ebb5360)

3. Select "Custom Networks"
   
![image](https://github.com/bitindi/docs/assets/119077822/0004266f-a4ab-44aa-9194-e599dd01bba0)

4. Add custom ETH Protect RPC to your Metamask
- Network Name:  ETH Protect
- RPC URL: [https://ethpro.bitindi.org](https://ethpro.bitindi.org) 
- Chain ID: 1
- Symbol: ETH
- Block Explorer URL (optional): https://etherscan.io

![spaces_-MEhQI8zckriC1VzHORZ_uploads_ifFMaCkPqazArnGHACqk_Screen Shot 2023-05-04 at 3](https://github.com/bitindi/docs/assets/119077822/fbd3f3a0-4f4c-4b76-9dd5-77918c2929d2)


# ETH Gas Protect RPC

ETH Gas Protect RPC combines front-running and gas protection to offer an all-in-one security solution for transactions on the Ethereum network. This RPC converts the private transaction to a single-transaction Flashbots bundle. By sending transactions directly to block proposers using our high-performance global network, ETH Gas Protect PRC eliminates the possibility of wasting gas on reverted transactions and keeps transactions hidden from front-running and sandwich bots until after the window of opportunity for an attack has passed. Traders can opt to use the ETH Protect RPC or the ETH Gas Protect RPC based on their use case.
Setup custom ETH Gas Protect RPC in Metamask
1. Open Metamask and click on "Settings"
2. Click on "Networks", and then click on "Add Network" on the Networks menu.
3. Select "Custom Networks"
4. Add custom ETH Gas Protect RPC to your Metamask
- Network Name:  ETH Gas Protect
- RPC URL: [https://eth.bitindi.org](https://eth.bitindi.org
- Chain ID: 1
- Symbol: ETH
- Block Explorer URL (optional): https://etherscan.io

# BSC Protect RPC

Front-running prevention public RPC adds a layer of privacy logic to route your transactions first to block proposers, stopping or delaying your transactions from appearing in the public mempool. This delay feature provides users opportunities to execute their trade before malicious front-running and sandwich bots can initiate attacks. Front-running prevention does not guarantee your transactions will not be attacked - your transaction info will eventually become public info.
The front-running prevention public RPC automatically routes your transaction to one of bitindi’s servers closest to your location. Use the RPC DNS https://bsc.bitindi.org to setup your wallet.
The limit rate is 3 transactions/sec. 
Setup custom BSC Protect RPC in Metamask
1. Open Metamask and click on "Settings"
2. Click on "Networks", and then click on "Add Network" on the Networks menu.
3. Select "Custom Networks"
4. Add custom BSC Protect RPC to your Metamask
- Network Name:  BSC Protect
- RPC URL: [https://bsc.bitindi.org](https://bsc.bitindi.org)
- Chain ID: 56
- Symbol: BNB
- Block Explorer URL (optional): https://bscscan.com

# Polygon Protect RPC

Front-running prevention public RPC adds a layer of privacy logic to route your transactions first to block proposers, stopping or delaying your transactions from appearing in the public mempool. This delay feature provides users opportunities to execute their trade before malicious front-running and sandwich bots can initiate attacks. Front-running prevention does not guarantee your transactions will not be attacked - your transaction info will eventually become public info.
The Front-running prevention public RPC automatically routes your transaction to one of bitindi’s servers closest to your location. Use the RPC DNS https://polygon.bitindi.org to setup your wallet.
Setup custom Polygon Protect RPC in Metamask
1. Open Metamask and click on "Settings"
2. Click on "Networks", and then click on "Add Network" on the Networks menu.
3. Select "Custom Networks"
4. Add custom Polygon Protect RPC to your Metamask
- Network Name:  Polygon Protect
- RPC URL: [https://polygon.bitindi.org](https://bsc.bitindi.org)
- Chain ID: 137
- Symbol: MATIC
- Block Explorer URL: https://polygonscan.com/
