# Inds getTransactionByHash

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getTransactionByHash" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getTransactionByHash", // jsonrpc method name
  "id": 1, // request id
  "jsonrpc": "2.0", // jsonrpc version
  "params": [
    "avalanche", // chain name
    "0x947022fc38f5c1c3349d0b2f77c82917ea3663141c535d07d674c1e21fd0c601", // tx_hash
  ]
}
```

Example Response

```json
{
  "jsonrpc": "2.0",
  "result": {
    "is_inscription": true,
    "transaction": {
      "protocol": "asc-20",
      "tick": "lobby",
      "deploy_hash": "0x947022fc38f5c1c3349d0b2f77c82917ea3663141c535d07d674c1e21fd0c601",
      "from": "0x7a7b6Be7f5Ac593bcb262b52ae5a731aa1690ad4",
      "to": "0x7a7b6Be7f5Ac593bcb262b52ae5a731aa1690ad4",
      "amount": "0"
    }
  },
  "id": 1
}
```

Curl Example&#x20;

```powershell
curl --location 'https://api.indexs.io/v2/rpc/inds_getTransactionByHash' \
--header 'Content-Type: application/json' \
--data '{
  "method": "inds_getTransactionByHash",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    "avalanche",
    "0x2f88df8669337ec739d8414df0f3ef32bf166cb73233c965e805b7fa54eef1f2"
  ]
}'
```
