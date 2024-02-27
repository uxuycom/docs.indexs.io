# Inds getBalancesByAddress

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getBalancesByAddress" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getBalancesByAddress", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    10, // page limit
    0, // page offset
    "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // address
    "", // chain name
    "", // protocol
    "" // tick name
    "" // key  exp: like "%key%"
    1  // sort  1:ASC 2:DESC
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
