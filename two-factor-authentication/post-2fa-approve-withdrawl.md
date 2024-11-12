---
description: Approve a withdrawal request by verifying the two-factor authentication code.
---

# \[POST] /2fa/approve-withdrawl

The \[POST]/2fa/approve-withdrawl method allows a withdrawal request to be approved after verifying the two-factor authentication (2FA) code provided by the user. It ensures that the user not only initiated the transaction but also has access to the authenticator device, adding a critical layer of security to the withdrawal process. By validating the temporary TOTP (Time-Based One-Time Password) code or another 2FA method, this method helps protect the account from unauthorized withdrawals by ensuring that only authenticated users can complete financial transactions.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

example:

```
{
  "userId": "user123",
  "token": "123456"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
