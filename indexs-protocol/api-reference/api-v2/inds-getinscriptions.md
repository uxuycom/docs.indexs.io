# Inds getInscriptions

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getInscriptions" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getInscriptions",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    10,  // page limit 
    0,   // page offset
    "",  // chain 
    "",  // protocol
    "",  // tick 
    "",  // deploy_by
    3   // sort : 0.default  1.deploy time  2.mint process  3.holders amt  4.transaction amt
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
                "chain": "btc",
                "protocol": "brc-20",
                "tick": "sats",
                "deploy_by": "bc1prtawdt82wfgrujx6d0heu0smxt4yykq440t447wan88csf3mc7csm3ulcn",
                "deploy_hash": "9b664bdd6f5ed80d8d88957b63364c41f3ad4efb8eee11366aa16435974d9333",
                "total_supply": "2100000000000000",
                "minted_percent": "1.0000",
                "limit_per_mint": "100000000",
                "holders": 1354607,
                "transfer_type": 0,
                "status": 2,
                "minted": "2100000000000000",
                "tx_cnt": 21192628,
                "created_at": 1707230059
            },
            ...
        ],
        "total": 96724,
        "limit": 10,
        "offset": 0
    },
    "id": 1
}
```
