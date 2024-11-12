---
description: Generates a deposit address specific to a blockchain network
---

# \[POST] /deposit/create

The \[POST] /deposit/create method generates a unique deposit address specific to a blockchain network, allowing the user to securely receive cryptocurrency. When prompted to generate an address, the system automatically creates a valid public address for the chosen blockchain network (such as Bitcoin, Ethereum, or others) that can be used for future deposits. This feature makes receiving funds easier by providing a convenient and secure way to manage incoming transactions, ensuring that deposits are sent to the correct address on the blockchain network.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To generate a deposit address, simply enter the network ID and then click "Execute".

**Parameters**

<table><thead><tr><th width="364">Name</th><th>Description</th></tr></thead><tbody><tr><td>networkId</td><td>ID of the blockchain network for which the deposit address will be generated</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
