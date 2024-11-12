---
description: >-
  Converts an amount in BRL(Real) to an equivalent amount in a specific
  cryptocurrency
---

# \[POST] /conversion/brl-to-crypto

The \[POST] /conversion/brl-to-crypto method converts an amount in Brazilian reais (BRL) to the equivalent amount in a specific cryptocurrency, such as USDT (Tether). This functionality is useful for users and applications that want to know the approximate purchase value of cryptocurrencies in local currency, facilitating transactions and real-time decision-making based on market quotes.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

example:

```
{
  "amount": 100,
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "originalAmountInBrl": 100,
  "cryptoAmount": 17.2608,
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum",
  "rateInfo": {
    "brlToUsdRate": 0.174,
    "cryptoToUsdRate": 1
  },
  "fee": "0.14",
  "finalAmountInUsd": "17.26"
}
```
{% endtab %}
{% endtabs %}
