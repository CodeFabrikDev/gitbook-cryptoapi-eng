---
description: Get details of a specific blockchain network
---

# \[GET] /blockchain-networks/{id}

The \[GET] /blockchain-networks/{id} method of our API allows you to consult detailed information about a specific blockchain network, providing crucial data about its configuration, status and characteristics. By entering the Network ID, you receive a complete set of information related to that blockchain, including technical parameters, current status, transaction fees, processing capacity and much more.&#x20;

This endpoint is ideal for developers and platforms that need to obtain precise details about a specific network in order to carry out integrations or monitor the performance of their transactions in real time. It is also useful for checking settings such as consensus, average block time, validation methods and compatibility with smart contracts.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To see the details of one of the available networks, simply enter the ID of the desired blockchain network and then click on “Execute”.

**Parameters**

| Name | Description           |
| ---- | --------------------- |
| id   | Blockchain network ID |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
```
{% endtab %}
{% endtabs %}
