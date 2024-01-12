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

# Running Indexer & API Server

## Running Indexer

Run UXUY Indexer with the command `indexer`. Specify how UXUY Indexer can reach BlockChain node and where to store the database in the previous chapter.

{% code lineNumbers="true" %}
```bash
/usr/local/bin/indexer -config=config.json
```
{% endcode %}

## Running JSON RPC API Server

Run UXUY JSON RPC API Server with the command `apiserver`. Specify how API Server can reach the database.

If you use the same database you can use the same config.json, you can use a Master-Slave modes to host your MySQL, and copy the `config.json` to a new `slave-db-config.json` and config the slave database for your apiserver.

{% code lineNumbers="true" %}
```bash
/usr/local/bin/apiserver -config=config.json
# /usr/local/bin/apiserver -config=slave-db-config.json
```
{% endcode %}

The default api server is hosting on `localhost:6583`. You can change it in your config file.



