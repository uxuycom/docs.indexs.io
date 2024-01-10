# Address.Balances

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="address.Balances" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "address.Balances", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    10, // page limit
    0, // page offset
    "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // address
    "", // chain name
    "", // protocol
    "", // tick name
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "inscriptions": [
            {
                "chain": "avalanche", // chain name
                "protocol": "asc-20", // protocol
                "tick": "crazydog", // tick name
                "address": "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // address
                "balance": "21000000", // address balance
                "deploy_hash": "0x2f88df8669337ec739d8414df0f3ef32bf166cb73233c965e805b7fa54eef1f2", // deploy hash
                "transfer_type": 1 // transfer type 1.by utxo hash 2.by balance
            }
        ],
        "total": 1, // total records count
        "limit": 10, // current request limit
        "offset": 0 // current request offset
    },
    "id": 1
}
```
