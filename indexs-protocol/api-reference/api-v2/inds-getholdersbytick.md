# Inds getHoldersByTick

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getHoldersByTick" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Exampple Request

```json
{
  "method": "inds_getHoldersByTick", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    10, // page limit
    0, // page offset
    "avalanche", // chain name
    "asc-20", // protocol
    "crazydog", // tick name
    1, // 1:ASC 2:DESC
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
                "chain": "avalanche",
                "protocol": "asc-20",
                "tick": "crazydog",
                "deploy_hash": "0x2f88df8669337ec739d8414df0f3ef32bf166cb73233c965e805b7fa54eef1f2",
                "address": "0xF2f9D2575023D320475ed7875FCDCB9b52787E59",
                "balance": "21000000",
                "total_supply": "21000000"
            }
        ],
        "total": 1,
        "limit": 10,
        "offset": 0
    },
    "id": 1
}
```
