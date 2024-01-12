# Inscription.Tick

{% swagger src="https://api.indexs.io/v1/docs/openapi.json" path="inscription.Tick" method="post" %}
[https://api.indexs.io/v1/docs/openapi.json](https://api.indexs.io/v1/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inscription.Tick", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    "avalanche", // chain name
    "asc-20", // protocol
    "crazydog" // tick name
  ]
}
```

Example Response

```json
// Some code
{
    "jsonrpc": "2.0",
    "result": {
        "chain": "avalanche", // chain name
        "protocol": "asc-20", // protocol
        "tick": "crazydog", // tick symbol
        "name": "crazydog", // tick name
        "limit_per_mint": "21000000", // limit per mint
        "deploy_by": "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // deployer address
        "total_supply": "21000000", // total supply
        "deploy_hash": "0x2f88df8669337ec739d8414df0f3ef32bf166cb73233c965e805b7fa54eef1f2", // deploy hash
        "deploy_time": 1704152964, // deploy time
        "transfer_type": 0, // transfer type 1.by utxo hash 2.by balance
        "created_at": 1704524337, // create time
        "updated_at": 1704524337, // update time
        "decimals": 0 // decimal precision
    },
    "id": 1
}
```
