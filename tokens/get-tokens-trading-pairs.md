---
description: >-
  Gets a list of all currency pairs that can be traded, with optional filtering
  for base and quote currencies.
---

# \[GET] /tokens/trading-pairs

The \[GET] /transaction-status/conversion method returns a complete list of all currency pairs available for trading, with the option to apply filters for base and quote currencies. By providing parameters such as the base currency (e.g. BTC, USDT) or quote currency (e.g. BRL or USD), users can refine their query to only get the pairs that meet their specific needs. This feature is essential for cryptocurrency exchanges and trading platforms, allowing traders and developers to access up-to-date information on available currency pairs and conduct transactions more efficiently and in a personalized way.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To filter the list of all currency pairs that can be traded, simply enter the base currency and the quote currency and then click on "Execute", if you want to see the full list, simply leave it blank.

**Parameters**

| Name  | Description                            |
| ----- | -------------------------------------- |
| base  | Base currency to filter trading pairs  |
| quote | Quote currency to filter trading pairs |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "id": "BAT-ETH",
    "base_currency": "BAT",
    "quote_currency": "ETH",
    "display_name": "BAT-ETH",
    "status": "online",
    "trading_disabled": false
  },
  {
    "id": "SYLO-USD",
    "base_currency": "SYLO",
    "quote_currency": "USD",
    "display_name": "SYLO-USD",
    "status": "delisted",
    "trading_disabled": true
  },
  {
    "id": "COMP-USD",
    "base_currency": "COMP",
    "quote_currency": "USD",
    "display_name": "COMP-USD",
    "status": "online",
    "trading_disabled": false
  },
  {
    "id": "ARKM-USD",
    "base_currency": "ARKM",
    "quote_currency": "USD",
    "display_name": "ARKM/USD",
    "status": "online",
    "trading_disabled": false
  }
  ]
```
{% endtab %}
{% endtabs %}
