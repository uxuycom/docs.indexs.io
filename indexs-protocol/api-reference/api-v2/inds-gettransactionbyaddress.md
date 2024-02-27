# Inds getTransactionByAddress

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getTransactionByAddress" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getTransactionByAddress", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    10, // page limit
    0, // page offset
    "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // address
    "", // chain name
    "", // protocol
    "", // tick name
    0, // event type : 1.deploy 2.mint 3.trans in 4.trans out
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "transactions": [
            {
                "chain": "avalanche", // chain
                "protocol": "asc-20", // protocol 
                "tick": "crazydog", // tick name
                "address": "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // address
                "tx_hash": "0xe89e1c445431a695fcc2797cde214a731c65765468e6095672fb0cbe8f8a6fdd", // tx hash
                "amount": "21000000", // tx amount
                "event": 2, // event type : 1.deploy 2.mint 3.trans in 4.trans out
                "operate": "mint", // operation name
                "created_at": 1704524337, // create time
                "updated_at": 1704524337 // update time
            }
        ],
        "total": 1,
        "limit": 10,
        "offset": 0
    },
    "id": 1
}
```
