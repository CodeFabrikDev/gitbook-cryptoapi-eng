---
description: Generates a TOTP secret for the user to configure two-factor authentication.
---

# \[POST] /2fa/generate

The \[POST]/2fa/generate method generates a TOTP (Time-Based One-Time Password) secret for the user, allowing them to set up two-factor authentication (2FA) on their account. The TOTP secret is a unique code that can be scanned in authenticator applications, such as Google Authenticator or Authy, to generate temporary authentication codes. This process adds an extra layer of security, requiring the user to enter an additional authentication code when logging in, in addition to the password, protecting the account from unauthorized access.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

example:

```
{
  "userId": "user123"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
