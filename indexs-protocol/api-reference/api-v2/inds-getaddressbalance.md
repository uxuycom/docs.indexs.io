# Inds getAddressBalance

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getAddressBalance" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getAddressBalance", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    "0xF2f9D2575023D320475ed7875FCDCB9b52787E59", // address
    "avalanche", // chain name
    "asc-20", // protocol
    "crazydog", // tick name
  ]
}
```

Example Response

```json
{
    "jsonrpc": "2.0",
    "result": {
        "tick": "crazydog", // tick name
        "balance": "5.0", // balance amount
        "transfer_type": 1 // transfer type 1.by utxo hash 2.by balance
    },
    "id": 1
}
```

Curl Example&#x20;

```powershell
curl --location 'https://api.indexs.io/v2/rpc/inds_getAddressBalance' \
--header 'Content-Type: application/json' \
--data '{
  "method": "inds_getAddressBalance",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    "0xF2f9D2575023D320475ed7875FCDCB9b52787E59",
    "avalanche",
    "asc-20",
    "crazydog"
  ]
}'
```
