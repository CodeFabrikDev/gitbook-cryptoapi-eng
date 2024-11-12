---
description: Authenticate and obtain a JWT token
---

# \[POST] /auth/login

The \[POST] /auth/login method authenticates the user's credentials and returns a JWT token (JSON Web Token) for secure access to the application's other protected endpoints. By submitting login credentials, such as email and password, the user receives a valid JWT token that can be used for authentication in subsequent calls, avoiding the need to re-present credentials. Using JWT provides a secure and efficient way to manage user sessions in distributed applications, ensuring that only authenticated users can access sensitive resources during the token's validity period.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

example:

```
{
  "username": "admin",
  "password": "password123"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InNkdmFsZSIsInN1YiI6MSwiaWF0IjoxNzMxMzMwMTU1LCJleHAiOjE3MzEzNTg5NTV9.8SzGYaLV4rTzXA70Rx4AhKdSxku0STA06zUcRNvp9A2"
}
```
{% endtab %}
{% endtabs %}
