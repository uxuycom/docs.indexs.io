# Block.LastNumber

{% swagger src="https://api.indexs.io/v1/docs/openapi.json" path="block.LastNumber" method="post" %}
[https://api.indexs.io/v1/docs/openapi.json](https://api.indexs.io/v1/docs/openapi.json)
{% endswagger %}

Example Request



```json
{
  "method": "block.LastNumber", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    ["avalanche"] // chain name array
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": [{
            "chain": "avalanche",
            "block_number": "40433785",
            "block_time": "2024-01-16 10:18:46 +0000 UTC",
            "timestamp": 1705400326
        }
    ],
    "id": 1
}
```
