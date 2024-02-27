# Inds getAllChains

{% swagger src="https://api.indexs.io/v2/docs/openapi.json" path="/inds_getAllChains" method="post" %}
[https://api.indexs.io/v2/docs/openapi.json](https://api.indexs.io/v2/docs/openapi.json)
{% endswagger %}

Example Request

```json
{
  "method": "inds_getAllChains",  
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    []    // chain 
  ]
}
```



Example Response

```json
{
    "jsonrpc": "2.0",
    "result": [
        {
            "chain_id": 1,
            "chain": "eth",
            "outer_chain": "eth",
            "name": "Ethereum",
            "logo": "https://s3.indexs.io/chain/icon/eth.png",
            "network_id": 1,
            "ext": "",
            "block_number": "19319706",
            "block_time": "2024-02-27T15:12:23Z",
            "timestamp": "2024-02-27T15:14:28Z"
        },
        {
            "chain_id": 43114,
            "chain": "avalanche",
            "outer_chain": "avax",
            "name": "Avalanche",
            "logo": "https://s3.indexs.io/chain/icon/avalanche.png",
            "network_id": 43114,
            "ext": "",
            "block_number": "42060612",
            "block_time": "2024-02-24T00:11:02Z",
            "timestamp": "2024-02-27T15:20:53Z"
        },
        {
            "chain_id": 42161,
            "chain": "arbitrum",
            "outer_chain": "ETH",
            "name": "Arbitrum One",
            "logo": "https://s3.indexs.io/chain/icon/arbitrum.png",
            "network_id": 42161,
            "ext": "",
            "block_number": "183652607",
            "block_time": "2024-02-23T11:44:17Z",
            "timestamp": "2024-02-23T11:44:22Z"
        },
        {
            "chain_id": 56,
            "chain": "bsc",
            "outer_chain": "BSC",
            "name": "BNB Smart Chain Mainnet",
            "logo": "https://s3.indexs.io/chain/icon/bsc.png",
            "network_id": 56,
            "ext": "",
            "block_number": "36505209",
            "block_time": "2024-02-27T15:15:54Z",
            "timestamp": "2024-02-27T15:16:26Z"
        },
        {
            "chain_id": 250,
            "chain": "fantom",
            "outer_chain": "FTM",
            "name": "Fantom Opera",
            "logo": "https://s3.indexs.io/chain/icon/fantom.png",
            "network_id": 250,
            "ext": "",
            "block_number": "76421555",
            "block_time": "2024-02-27T14:42:35Z",
            "timestamp": "2024-02-27T14:43:09Z"
        },
        {
            "chain_id": 137,
            "chain": "polygon",
            "outer_chain": "Polygon",
            "name": "Polygon Mainnet",
            "logo": "https://s3.indexs.io/chain/icon/polygon.png",
            "network_id": 137,
            "ext": "",
            "block_number": "54023873",
            "block_time": "2024-02-27T15:13:42Z",
            "timestamp": "2024-02-27T15:14:24Z"
        },
        {
            "chain_id": 0,
            "chain": "btc",
            "outer_chain": "btc",
            "name": "BTC",
            "logo": "https://s3.indexs.io/chain/icon/btc.png",
            "network_id": 0,
            "ext": "",
            "block_number": "830439",
            "block_time": "2024-02-14T15:33:22Z",
            "timestamp": "2024-02-14T15:55:39Z"
        }
    ],
    "id": 1
}
```
