---
description: Get the quote for a specific currency pair
---

# \[GET] /exchange-rates/pair

The \[GET] /exchange-rates/pair method of our API allows you to consult the current value of a specific cryptocurrency pair, such as BTCUSD, ETHUSD, among others. This endpoint provides real-time information on the price of various currency pairs, allowing you to integrate market data directly into your application, e-commerce platform or financial service.&#x20;

With this feature, it is possible to obtain the rate of a specific currency pair in different units of measurement, such as the value in US dollars (USD), euros (EUR), or other fiat and digital currencies. The method returns accurate information on the buying and selling price, as well as the price change over a given period, helping you to make informed decisions about transactions and investments.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To get the quote for a specific currency pair, simply enter the ID of the desired cryptocurrency (e.g. bitcoin, ethereum, etc.) and the currency it will be quoted against (e.g. usd, brl), then click “Execute”.

**Parameters**

| Name       | Description                                              |
| ---------- | -------------------------------------------------------- |
| cryptold   | Cryptocurrency ID according to CoinGecko                 |
| vcCurrency | Currency against which the cryptocurrency will be quoted |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "cryptoId": "bitcoin",
  "vsCurrency": "usd",
  "price": 82274
}
```
{% endtab %}
{% endtabs %}
