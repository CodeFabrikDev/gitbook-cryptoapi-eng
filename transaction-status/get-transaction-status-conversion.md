---
description: Check the status of a currency conversion transaction by transaction ID
---

# \[GET] /transaction-status/conversion

The \[GET] /transaction-status/conversion method allows you to check the status of a cryptocurrency conversion transaction using the transaction ID. By providing the unique transaction ID, the method returns detailed information about the progress of the conversion, such as whether the transaction has completed, is pending, or has failed. This feature is useful for platforms that want to monitor and provide real-time updates to users on the status of their cryptocurrency conversions, providing transparency and making it easier to track ongoing financial processes.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To check the status of a conversion transaction, simply enter the transaction ID and then click "Execute".

**Parameters**

| Name          | Description                               |
| ------------- | ----------------------------------------- |
| transactionId | Conversion transaction ID to check status |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "transactionId": "TX123456",
  "status": "Completed"
}
```
{% endtab %}
{% endtabs %}
