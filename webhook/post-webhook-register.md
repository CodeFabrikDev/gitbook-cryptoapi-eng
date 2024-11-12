---
description: Register a new webhook associated with a specific withdrawal transaction
---

# \[POST] /webhook/register

The \[POST] /webhook/register method allows you to register a new webhook associated with a specific withdrawal transaction. By configuring the webhook, the user can receive real-time notifications about the status of a withdrawal transaction, such as confirmations, processing or completion. This functionality is ideal for developers and platforms that want to automatically monitor the progress of transactions and integrate instant notifications into their systems, making it easier to track and automate actions related to cryptocurrency withdrawals.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

example:

```
{
  "url": "https://meusite.com/webhook",
  "transactionId": "TX123456"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "id": 1,
  "url": "https://meusite.com/webhook",
  "transactionId": "TX123456"
}
```
{% endtab %}
{% endtabs %}
