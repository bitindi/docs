---
title: "Compile and Run"
description: "Bitindi chain Install"
lead: "Install your Bitindi chain Node."
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

### Download
Download source code via [git](https://github.com/Bitindi/bitindi-Core.git)

`git clone https://github.com/Bitindi/bitindi-Core.git`

 `Install Golang Reference`: [Go Download and install](https://go.dev/doc/install)

## Compile

```
cd /path/to/bitindi 
make geth
```
If you want to use cross compile, like compiling on `Mac` for `Linux`, use `make geth-linux`, `make geth-linux-amd64`, etc.

After compilation completed, the generated binary is in the folder `build/bin`

## Run
By running ./build/bin/geth --help, we can get all option info. Specific usage can refer to [Command-line](https://geth.ethereum.org/docs/interface/command-line-options) Options

## Deployment
please refer [deployment](/docs/developers/deploy/)

*SSD is required*

## Network
Program will connect into `mainnet` after started. If want to connect the public testnet, you can add option `--testnet` to command when starting.