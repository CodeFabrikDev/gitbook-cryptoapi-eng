---
description: Returns a list of all registered webhooks
---

# \[GET] /webhook/list

The \[GET] /webhook/list method returns a complete list of all the webhooks registered by the user.

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
    "url": "https://meusite.com/webhook",
    "transactionId": "TX123456"
  }
]
```
{% endtab %}
{% endtabs %}
