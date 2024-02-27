# Inds getTransactions

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getTransactions" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getTransactions",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    10, // page limit
    0, // page offset
    "", // address
    "", // chain
    "",  // protocol 
    "", // tick 
    1   // sortmode 1:ASC 2:DESC
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "data": [
            {
                "id": 1,
                "chain": "avalanche",
                "protocol": "",
                "block_height": 31918263,
                "position_in_block": 8,
                "block_time": "2023-06-28T16:17:05Z",
                "tx_hash": "7ffc56b2bf20f4f3474c1fd503fc3f1fb9066c8b0665d6da11185cac892108a5",
                "from": "0xE0eCCFe34c367Cbe0b6B261011b6781229942552",
                "to": "0xE0eCCFe34c367Cbe0b6B261011b6781229942552",
                "op": "",
                "tick": "",
                "amt": "0",
                "gas": 22248,
                "gas_price": 26500000000,
                "status": 0,
                "created_at": "2024-01-15T09:37:29Z",
                "updated_at": "2024-01-15T09:37:29Z"
            },
            ...
         
        ],
        "total": 0,
        "limit": 10,
        "offset": 0,
        "code": 0,
        "msg": 0
    },
    "id": 1
}
```
