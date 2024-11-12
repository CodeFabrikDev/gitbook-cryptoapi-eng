---
description: List all deposit addresses generated for each blockchain network
---

# \[GET] /deposit/list

The \[GET] /deposit/list method returns a list of all deposit addresses generated for each blockchain network associated with the user’s account. It provides a centralized view of public addresses, allowing users to easily see which addresses specific to each network (such as Bitcoin, Ethereum, etc.) they can receive deposits to. This functionality is useful for platforms that manage multiple cryptocurrencies and want to make it easier to track active addresses, ensuring that transactions are sent to the correct locations on the blockchain network.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To list all generated deposits, just click on "Execute".

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "networkId": 1,
    "networkName": "Ethereum",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 2,
    "networkName": "Binance Smart Chain",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 3,
    "networkName": "Polygon",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 4,
    "networkName": "Avalanche",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  }
]
```
{% endtab %}
{% endtabs %}
