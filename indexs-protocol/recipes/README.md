---
cover: ../../.gitbook/assets/gitbook-background-664X240 (1).png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Recipes

## DMT Spirit

DMT Spirit is based on Deploy, Mint, Transfer Operation and inscribe the OP behavior on blockchain.

This means fair mint, every user can get the assets in fair chance, there will not be any project owner, the assets economics based on community.

```json
// Example
Deploy: 
{ 
    "p": "brc-20", 
    "op": "deploy", 
    "tick": "publish0xtoken", 
    "max": "2100000", 
    "lim": "1000" 
}

Mint: 
{ 
    "p": "brc-20", 
    "op": "mint", 
    "tick": "publish0xtoken", 
    "amt": "1000" 
}

Transfer: 
{
    "p": "brc-20", 
    "op": "transfer", 
    "tick": "publish0xtoken", 
    "amt": "10" 
}
```

## Deploy

```
// Some code
{ 
    "p": "brc-20", 
    "op": "deploy", 
    "tick": "publish0xtoken", 
    "max": "2100000", 
    "lim": "1000" 
}
```

## Mint

```
// Some code
{ 
    "p": "brc-20", 
    "op": "mint", 
    "tick": "publish0xtoken", 
    "amt": "1000" 
}
```

## Transfer

## BRC20 style

BRC20 style inscriptions use the follow data and UTXO to inscribe the transfer event on blockchain.

```json
// Transfer
{ 
    "p": "brc-20", 
    "op": "transfer", 
    "tick": "ordi", 
    "amt": "10" 
}

```

## Ethscription

[https://docs.ethscriptions.com/esips/accepted-esips/esip-1-smart-contract-ethscription-transfers](https://docs.ethscriptions.com/esips/accepted-esips/esip-1-smart-contract-ethscription-transfers)

&#x20;                                                                  Ethscription Transfer Policy
