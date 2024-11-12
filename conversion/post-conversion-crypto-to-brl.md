---
description: Convert a specific amount of cryptocurrency to BRL
---

# \[POST] /conversion/crypto-to-brl

The \[POST] /conversion/crypto-to-brl method converts a specific amount of a cryptocurrency, such as BTC (Bitcoin) or USDT (Tether), to the equivalent value in BRL (Brazilian real). When providing the desired amount of cryptocurrency, the method returns the corresponding value in BRL, based on the current market price. This feature is useful for applications that need to display the value of cryptocurrencies in local currency, helping users visualize the value of their digital assets in reais, which facilitates transactions, calculations and financial decision-making.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

example:

```
{
  "cryptoAmount": 0.5,
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
  "cryptoAmount": 0.5,
  "equivalentBrl": "2.85",
  "fee": "0.00",
  "finalAmountInUsd": "0.50",
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum",
  "rateInfo": {
    "brlToUsdRate": 0.174,
    "cryptoToUsdRate": 1
  }
}
```
{% endtab %}
{% endtabs %}
