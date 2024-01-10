# Tool.InscriptionTxOperate

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="tool.InscriptionTxOperate" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "tool.InscriptionTxOperate", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    "avalanche", // chain name
    "646174613a2c7b2270223a226173632d3230222c226f70223a226d696e74222c227469636b223a22746f6d726179222c22616d74223a2231227d", // input data
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0", // jsonrpc version
    "result": {
        "operate": "mint", // operation name
        "protocol": "asc-20", // protocol
        "tick": "tomray" // tick name
    },
    "id": 1 // current request id
}
```
