---
title: "BIP20 Token Standard"
description: "BIP20 Token Standard"
lead: "Bitindi is fully compatible with ERC20 standard，interfaces and events as follows："
date: 2022-10-06T08:48:57+00:00
lastmod: 2022-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "users"
weight: 120
toc: true
---

```
// ----------------------------------------------------------------------------
// ERC Token Standard #20 Interface
// https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20-token-standard.md
// ----------------------------------------------------------------------------
contract ERC20Interface {
    function totalSupply() public constant returns (uint);
    function balanceOf(address tokenOwner) public constant returns (uint balance);
    function allowance(address tokenOwner, address spender) public constant returns (uint remaining);
    function transfer(address to, uint tokens) public returns (bool success);
    function approve(address spender, uint tokens) public returns (bool success);
    function transferFrom(address from, address to, uint tokens) public returns (bool success);

    event Transfer(address indexed from, address indexed to, uint tokens);
    event Approval(address indexed tokenOwner, address indexed spender, uint tokens);
}
```
### EIP reference：

[eip-20](https://eips.ethereum.org/EIPS/eip-20)

### Implemetation reference：

[openzeppelin-contracts](https://github.com/OpenZeppelin/openzeppelin-contracts/tree/master/contracts/token/ERC20)
```