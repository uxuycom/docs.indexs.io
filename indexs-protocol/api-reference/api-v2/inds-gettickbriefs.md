# Inds getTickBriefs

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getTickBriefs" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

````json
{
 "method": "inds_getTickBriefs", // jsonrpc method name
 "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    [
      {
        "chain": "avalanche",  // chain 
        "deploy_hash": "0x7ffc56b2bf20f4f3474c1fd503fc3f1fb9066c8b0665d6da11185cac892108a5"  // ```postman_json
deploy_hash
```
      }
    ]
  ]
}

````

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "inscriptions": [
            {
                "id": 0,
                "chain": "avalanche",
                "protocol": "asc-20",
                "tick": "avas",
                "name": "avas",
                "limit_per_mint": "1000",
                "deploy_by": "0xE0eCCFe34c367Cbe0b6B261011b6781229942552",
                "total_supply": "21000000",
                "deploy_hash": "0x7ffc56b2bf20f4f3474c1fd503fc3f1fb9066c8b0665d6da11185cac892108a5",
                "deploy_time": "2023-06-28T16:17:05Z",
                "transfer_type": 0,
                "created_at": "2024-01-15T09:37:29Z",
                "updated_at": "0001-01-01T00:00:00Z",
                "decimals": 0,
                "holders": 5195,
                "minted": "21000000",
                "tx_cnt": 54446,
                "progress": "0"
            }
        ]
    },
    "id": 1
}
```

Curl Example&#x20;

```powershell
curl --location 'https://api.indexs.io/v2/rpc/inds_getTickBriefs' \
--header 'Content-Type: application/json' \
--data '{
  "method": "inds_getTickBriefs",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    [
      {
        "chain": "avalanche",
        "deploy_hash": "0x7ffc56b2bf20f4f3474c1fd503fc3f1fb9066c8b0665d6da11185cac892108a5"
      }
    ]
  ]
}'

```
