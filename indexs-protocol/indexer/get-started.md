---
description: >-
  The UXUY Indexer implements the inscription protocol on the blockchain and
  index the data from all blockchain.
---

# Get Started

***

> ### careful
>
> UXUY Indexer is alpha software. Use it on mainnet at your own risk!



## Prerequisites

UXUY Indexer requires `golang` if you want to compiled from source.&#x20;

{% code lineNumbers="true" %}
```bash
// Mac
wget -c https://go.dev/dl/go1.21.6.darwin-amd64.tar.gz -O \
    - | sudo tar -xz -C /usr/local

// Linux
wget -c https://go.dev/dl/go1.21.6.linux-amd64.tar.gz -O \ 
    - | sudo tar -xz -C /usr/local
    
export PATH=$PATH:/usr/local/go/bin

```
{% endcode %}

UXUY Indexer need to store index data in your database, so far we support mySQL and will support SQLite. you need to install MySQL in your machine or config your MySQL connect info follow the next chapter.



## Installation

### From source:

Compile UXUY Indexer from source by cloning the uxuy indexer repository. Go Version 1.21 or higher is recommended (you may check what version of go is running with `go version`)

```
git clone https://github.com/uxuycom/indexer.git
cd indexer
checkout <latest version>
make install
```
