---
title: "Add  RPC"
description: "Add a Network or Custom RPC"

---


<!--more-->

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Adding blockchain to Metamask</title>
  </head>
  <body>
    <script>
      // FUSE blockchain details
      const chainId = '0x7a';
      const rpcURL = 'https://rpc.fuse.io';
      const networkName = 'Fuse Mainnet';
      const currencyName = 'FUSE';
      const currencySymbol = 'FUSE';
      const explorerURL = 'https://explorer.fuse.io/';

      const addNetwork = async () => {
        if (!window.ethereum) {
          console.error('Metamask not detected');
          return;
        }
        await window.ethereum.request({
          method: 'wallet_addEthereumChain',
          params: [
            {
              chainId: chainId,
              chainName: networkName,
              rpcUrls: [rpcURL],
              blockExplorerUrls: [explorerURL],

              nativeCurrency: {
                name: currencyName,
                symbol: currencySymbol, // 2-6 characters long
                decimals: 18,
              },
            },
          ],
        });
        // refresh
        window.location.reload();
      };
    </script>
    <!-- The button  -->
    <button onClick="addNetwork()">Add Fuse</button>
  </body>
</html>