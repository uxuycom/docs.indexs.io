# Inds getTickByCallData

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getTickByCallData" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getTickByCallData", // jsonrpc method name
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

Curl Example&#x20;

```powershell
curl --location 'https://api.indexs.io/v2/rpc/inds_getTickByCallData' \
--header 'Content-Type: application/json' \
--data '{
  "method": "inds_getTickByCallData",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    "avalanche",
    "0x646174613a2c7b2270223a226173632d3230222c226f70223a226d696e74222c227469636b223a22746f6d726179222c22616d74223a2231227d"
  ]
}'
```
