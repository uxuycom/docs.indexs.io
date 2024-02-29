# Inds getLastBlockNumberIndexed

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getLastBlockNumberIndexed" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getLastBlockNumberIndexed", // jsonrpc method name
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

Curl Example&#x20;

```powershell
curl --location 'https://api.indexs.io/v2/rpc/inds_getLastBlockNumberIndexed' \
--header 'Content-Type: application/json' \
--data '{
  "method": "inds_getLastBlockNumberIndexed",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    [
      "avalanche"
    ]
  ]
}'
```
