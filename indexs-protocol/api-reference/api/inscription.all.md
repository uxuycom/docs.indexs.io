# Inscription.All

{% swagger src="https://api.indexs.io/v1/docs/openapi.json" path="inscription.All" method="post" %}
[https://api.indexs.io/v1/docs/openapi.json](https://api.indexs.io/v1/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inscription.All", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    10, // page limit
    0, // page offset
    "", // chhain name
    "", // protocol
    "", // tick name
    "", // deployer address
    0,  // sort : 0.default  1.deploy time  2.mint process  3.holders amt  4.transaction amt
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0", // jsonrpc version
    "result": {
        "inscriptions": [
            {
                "chain": "polygon", // chain name
                "protocol": "brc-20", // protocol
                "tick": "ggang", // tick name
                "deploy_by": "0x53B4daF4a49bB1a91D8Adfca584529f69e5211F5", // deployer address
                "deploy_hash": "0x0a2672352f59b27b29a2cbbd043930441daed984af2a73cd94e2ee2d77e9041c", // deploy hash
                "total_supply": "5000", // total supply
                "minted_percent": "0.5000", // minted percent
                "limit_per_mint": "500", // limit for per mint
                "holders": 2, // holders amount
                "transfer_type": 0, // transfer type : 1.by utxo hash 2.by balance
                "status": 1, // status 
                "minted": "2500", // minted count
                "tx_cnt": 6, // transactions count
                "created_at": 1704532932 // create time
            }
        ],
        "total": 347, // total records number
        "limit": 1, // current request page limit
        "offset": 0 // current request page offset
    },
    "id": 1 // request id
}
```
