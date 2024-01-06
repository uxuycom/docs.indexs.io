# Quick Start

So far, UXUY Indexer has opensource and release alpha version.



{% embed url="https://github.com/uxuycom/indexer" %}

### Standalone

The `UXUY` Indexer has two parts, the first part is `Indexer` and the second one is `API-Server`.&#x20;

Indexer has 3 modules, `Scan` `Index` `Persistent.`

### Prepare

#### Depends

* You need to know golang, mysql, linux and some tech stack knowledge.
* Have a valid RPC Endpoint for you want to index the EVM blockchain.
* MySQL Database on your server or cloud.

#### Build & Run

{% code lineNumbers="true" %}
```bash
git clone https://github.com/uxuycom/indexer.git
cd indexer/db
mysql -uroot -p < indexer-init.sql
```
{% endcode %}

{% code overflow="wrap" lineNumbers="true" %}
```bash
// RUN Indexer
git clone https://github.com/uxuycom/indexer.git
cd indexer
make build-indexer

cp config.json.template config.json

// Before do this, you needs to initial database first.
// mysql 
// Update the config follow the docs


./indexer -c config.json
```
{% endcode %}

When Indexer worked, you can check the data in your database. if it works normal, you can going to run API Server.

{% code lineNumbers="true" %}
```bash
// Run Indexer JSONRPC API
git clone https://github.com/uxuycom/indexer.git
cd indexer
make build-indexer-api

cp apis-config.json.template apis-config.json
// Update the config follow the docs
./indexer-api -c apis-config.json
```
{% endcode %}

### Docker

You can run `Indexer` and `API` use Docker too.



### How to contrib. ?

If you are a developer, you can join us to develop and make the indexer more powerful.

If you are interesting on this, feel free to join the community to make better place.

