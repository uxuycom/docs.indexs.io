---
description: UXUY Indexer OpenAPI, We provide the OpenAPI alpha version now.
cover: ../../.gitbook/assets/gitbook-background-664X240 (1).png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# API Reference

## Introduction

***

The UXUY JSON-RPC API is the canonical interface between users and the Indexer. Each execution layer client implements the API as defined by the spec.

As the main source of chain information, anything that is not provided over via API will not be easily accessible to users.



## Guiding Principles

***

## OPENAPI

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="inscription.All" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="inscription.Tick" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="address.Transactions" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="address.Balances" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="address.Balance" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="tick.Holders" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="block.LastNumber" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

{% swagger src="https://ava.indexs.io/v1/docs/openapi.json" path="tool.InscriptionTxOperate" method="post" %}
[https://ava.indexs.io/v1/docs/openapi.json](https://ava.indexs.io/v1/docs/openapi.json)
{% endswagger %}

## JSON-RPC methods

* [inscription.All](./#inscription.all)
* [inscription.Tick](./#inscription.tick)
* address.Transactions
* address.Balances
* address.Balance
* tick.Holders
* block.LastNumber

## JSON-RPC API Reference

### inscription.All

Return all inscriptions

#### Parameters

<pre class="language-json"><code class="lang-json">// Some code
type FindAllInscriptionsCmd struct {
	Limit    int    `json:"limit"`
	Offset   int    `json:"offset"`
	Chain    string `json:"chain"`
	Protocol string `json:"protocol"`
	Tick     string `json:"tick"`
	DeployBy string `json:"deploy_by"`
	Sort     int    `json:"sort"`
}

<strong>{
</strong>  "method": "inscription.All",
  "id": 1,
  "jsonrpc": "2.0",
  "params": [
    10,  
    0,
    "",
    "",
    "aval",
    "",
    0
  ]
}
</code></pre>

#### Returns

```
// Some code
```

#### Example

Request

```
// Some code
```

Response

```
// Some code
```

### inscription.Tick

Return Single Inscription

#### Parameters

```json
// Some code
"params": [

]
```

#### Returns

```
// Some code
```

#### Example

Request

```
// Some code
```

Response

```
// Some code
```

```
```





