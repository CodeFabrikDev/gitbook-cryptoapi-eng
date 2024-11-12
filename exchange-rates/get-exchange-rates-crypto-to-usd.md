---
description: Get the rate of a cryptocurrency to USD(Dollar)
---

# \[GET] /exchange-rates/crypto-to-usd

The \[GET] /exchange-rates/crypto-to-usd method makes it possible to obtain the current rate of a specific cryptocurrency, such as Bitcoin (BTC), in relation to the US dollar (USD). It queries real-time data from financial markets and returns the most recent conversion value between the cryptocurrency and the USD, enabling applications and users to track price changes and make informed decisions in their transactions.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To get the rate of a cryptocurrency to USD, simply enter the ID of the cryptocurrency you want (e.g. BTC, ETH, etc.) and then click on “Execute”.

**Parameters**

| Name         | Description           |
| ------------ | --------------------- |
| cryptoSymbol | Cryptocurrency symbol |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "cryptoId": "bitcoin",
  "vsCurrency": "usd",
  "price": 82194
}
```
{% endtab %}
{% endtabs %}
