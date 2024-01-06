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
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Transfer

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

{% embed url="https://docs.ethscriptions.com/esips/accepted-esips/esip-1-smart-contract-ethscription-transfers" %}
Ethscription Transfer Policy
{% endembed %}

