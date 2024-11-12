---
description: Get the rate of a cryptocurrency to BRL(Real)
---

# \[GET] /exchange-rates/crypto-to-brl

The \[GET] /exchange-rates/crypto-to-brl method makes it possible to obtain the current rate of a specific cryptocurrency, such as Bitcoin (BTC), in relation to the Brazilian real (BRL). It queries real-time data from financial markets and returns the most recent conversion value between the cryptocurrency and the BRL, enabling applications and users to track price changes and make informed decisions in their transactions.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To get the rate of a cryptocurrency for BRL, just enter the ID of the cryptocurrency you want (e.g. BTC, ETH, etc.) and then click on “Execute”.

**Parameters**

| Name         | Description           |
| ------------ | --------------------- |
| cryptoSymbol | Cryptocurrency symbol |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "symbol": "BTCBRL",
  "price": 475081.32000000007
}
```
{% endtab %}
{% endtabs %}
