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
    "avalanche", // chain name
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "block_number": 40007422 // last block number
    },
    "id": 1
}
```
