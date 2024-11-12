---
description: List all available blockchain networks
---

# \[GET] /blockchain-networks

The \[GET]/blockchain-networks method of our API allows you to access and consult the blockchain networks supported for integration into your application. With this endpoint, you can get a complete list of the main blockchain networks available for transactions.&#x20;

This feature is ideal for developers looking to identify the networks compatible with their platform or application, making it easier to choose the most suitable blockchain for the type of transaction or service they want to implement. The API provides detailed information about each network, such as its name, ChainID (network code) and deposit address.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

Just click on “Execute” to use the method.

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "id": 1,
    "name": "Ethereum",
    "chainId": "1",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 2,
    "name": "Binance Smart Chain",
    "chainId": "56",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 3,
    "name": "Polygon",
    "chainId": "137",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 4,
    "name": "Avalanche",
    "chainId": "43114",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  }
]
```
{% endtab %}
{% endtabs %}
