# Tick.Holders

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="tick.Holders" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "tick.Holders", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    10, // page limit
    0, // page offset
    "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // address
    "avalanche", // chain name
    "asc-20", // protocol
    "crazydog", // tick name
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "holders": [
            {
                "chain": "avalanche", // chain name
                "protocol": "asc-20", // protocol 
                "tick": "crazydog", // tick name
                "address": "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // holder address
                "balance": "21000000", // holder balance
                "deploy_hash": "", // deploy hash
                "transfer_type": 0 // transfer type 1.by utxo hash 2.by balance
            }
        ],
        "total": 1, // total records count
        "limit": 10, // current request limit
        "offset": 0 // current request offset
    },
    "id": 1
}
```
