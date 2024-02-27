# Inds search

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_search" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_search",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    "0x4273173187f1108007b1C1ABE5301eFa03f7fc8A",  // keyword 
    ""          // chain 
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "type": "Address",
        "data": [
            {
                "chain": "avalanche",
                "address": "0x4273173187f1108007b1C1ABE5301eFa03f7fc8A",
                "balance": "2613"
            },
            {
                "chain": "bsc",
                "address": "0x4273173187f1108007b1C1ABE5301eFa03f7fc8A",
                "balance": "1140"
            }
        ]
    },
    "id": 1
}
```
