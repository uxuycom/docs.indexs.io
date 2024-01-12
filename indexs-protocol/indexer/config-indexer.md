---
cover: ../../.gitbook/assets/gitbook-background-664X240 (1).png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Configuration

## How to config?

~~Optionally, we use a configuration file under `~/.uxuyindexer/config.json` on Linux or BSD, `~/Library/Application Support/uxuyindexer/config.json` in Mac OS or `$LOCALAPPDATA/uxuyindexer/config.json` in Windows.~~

You can set the config by self when you start it in command line too.&#x20;

The following is the config.json example.

### from\_block

It is very important when you want to index the data from blockchain, firstly you need to set a start time, here we use block height, I will give a example how to get the data.

You will know some ticks from your friends, community or others, now get the `deployed hash` from your information source, then go to the blockchain scan, such as&#x20;

{% embed url="https://avascan.info/blockchain/c/home" %}

You can use `snowtrace` to get the avas deploy info by the `hash` .

[https://snowtrace.io/tx/0x7ffc56b2bf20f4f3474c1fd503fc3f1fb9066c8b0665d6da11185cac892108a5](https://snowtrace.io/tx/0x7ffc56b2bf20f4f3474c1fd503fc3f1fb9066c8b0665d6da11185cac892108a5)

{% embed url="https://snowtrace.io/tx/0x7ffc56b2bf20f4f3474c1fd503fc3f1fb9066c8b0665d6da11185cac892108a5" %}

```
Block 31918263 -- This is the block height, you can use this in your config.
IDM:data:,{"p":"asc-20","op":"deploy","tick":"avas","max":"21000000","lim":"1000"}
```

### scan\_limit



### delayed\_scan\_number



### chain\_name

###

### rpc

###

### filters.event\_topics



### config.json

{% code lineNumbers="true" fullWidth="false" %}
```json
{
  "server": {
    "from_block": 40146071,
    "scan_limit": 1,
    "delayed_scan_number": 10
  },
  "database": {
    "type": "mysql",
    "dsn": "root:@tcp(127.0.0.1:3306)/tap_indexer?charset=utf8mb4&parseTime=True&loc=Local&collation=utf8mb4_general_ci",
    "enable_log": false
  },
  "chain": {
    "chain_name": "avalanche",
    "rpc": "https://1rpc.io/avax/c",
    "username": "",
    "password": ""
  },
  "log_level": "info",
  "notls": true,
  "rpclisten": [
    ":6583"
  ],
  "rpcmaxclients": 10000,
  "filters": {
    "event_topics": [
      "0xe2750d6418e3719830794d3db788aa72febcd657bcd18ed8f1facdbf61a69a9a",
      "0x3efe873bf4d1c1061b9980e7aed9b564e024844522ec8c80aec160809948ef77",
      "0x8cdf9e10a7b20e7a9c4e778fc3eb28f2766e438a9856a62eac39fbd2be98cbc2"
    ]
  },
  "profile_enabled": true
}
```
{% endcode %}
