# Quick Start

So far, UXUY Indexer has opensource and release alpha version.



{% embed url="https://github.com/uxuycom/indexer" %}

### Standalone

The `UXUY` Indexer has two parts, the first part is `Indexer` and the second one is `API-Server`.&#x20;

Indexer has 3 modules, `Scan` `Index` `Persistent.`



### Prerequisites:

* Ensure Golang is installed.
* Set up your Go workspace.

**Blockchain Indexer Setup:**

1. Choose or deploy an Ethereum node; obtain its RPC endpoint (e.g., Infura).
2. Set up MySQL on your server or use a cloud service.

#### Build & Run

{% code lineNumbers="true" %}
```bash
git clone https://github.com/uxuycom/indexer.git
mysql -uroot -p < indexer/db/init_mysql.sql
```
{% endcode %}

{% code overflow="wrap" lineNumbers="true" %}
```bash
// RUN Indexer
git clone https://github.com/uxuycom/indexer.git
cd indexer
make build && sudo make install

// Before do this, you needs to initial database first.
// mysql 
// Update the config follow the docs
indexer -c config.json

// Run Indexer JSONRPC API server
apiserver -c config.json
```
{% endcode %}

### Docker

You can run `Indexer` and `API` use Docker soon.

### How to become contributor ?

If you are a developer, you can join us to develop and make the indexer more powerful.

If you are interesting on this, feel free to join the community to make better place.

