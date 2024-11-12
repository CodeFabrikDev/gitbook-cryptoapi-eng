---
description: Gets the current transaction fees for a specific coin in the mempool.
---

# \[GET] /transaction-fee/single

The \[GET]/transaction-fee/single method displays the current transaction fees for a specific coin in the mempool, which is the set of pending transactions awaiting confirmation on the blockchain network. When querying the fees for a specific coin, such as BTC or ETH, the method returns real-time information on the average, minimum, and maximum fees, helping users adjust their transactions for faster confirmation or more cost-effective fees. This functionality is essential for users and platforms that want to optimize the cost and speed of their transactions by providing accurate and up-to-date data on congestion and transaction costs on their chosen blockchain network.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To check the rate of a currency, just enter the currency and then click "Execute".

**Parameters**

| Name     | Description             |
| -------- | ----------------------- |
| currency | Blockchain network code |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "currency": "BTC",
  "fastest_fee_usd": 9.71,
  "normal_fee_usd": 2.52,
  "slow_fee_usd": 4.49
}
```
{% endtab %}
{% endtabs %}
