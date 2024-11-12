---
description: >-
  Gets the current transaction fees for a currency pair (base and quote) in the
  mempool.
---

# \[GET] /transaction-fee/pair

The \[GET] /transaction-fee/pair method retrieves the current transaction fees for a specific currency pair (base currency and quote currency) from the mempool, where transactions are waiting to be processed on the blockchain network. By specifying the currency pair, such as BTC/USDT or ETH/BRL, the method returns real-time transaction fee data for conversions between these currencies, including average, minimum, and maximum fees. This feature is useful for users and platforms that want to track transaction fees between specific pairs, allowing them to adjust their operations based on current congestion conditions and costs on the blockchain.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To check the status of a conversion transaction, simply enter the transaction ID and then click "Execute".

**Parameters**

<table><thead><tr><th width="364">Name</th><th>Description</th></tr></thead><tbody><tr><td>base</td><td>Base currency code</td></tr><tr><td>quote</td><td>Quote currency code</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "base": {
    "currency": "BTC",
    "fastest_fee_usd": 8.49,
    "normal_fee_usd": 2.52,
    "slow_fee_usd": 7.77
  },
  "quote": {
    "currency": "ETH",
    "fastest_fee_usd": 4.28,
    "normal_fee_usd": 3.78,
    "slow_fee_usd": 3.04
  }
}
```
{% endtab %}
{% endtabs %}
