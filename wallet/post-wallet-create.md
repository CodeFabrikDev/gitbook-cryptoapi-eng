---
description: Blockchain Wallet Creation
---

# \[POST] /wallet/create

The \[POST] /wallet/create method allows the creation of a new blockchain wallet, linked to the user’s account. The generated wallet includes a unique public address, used to securely store and transact cryptocurrencies. This endpoint facilitates the management of digital assets by automatically creating a wallet that can receive deposits, perform withdrawals, and monitor balances in real time. Ideal for platforms that want to provide individual wallets to their users, this method provides a secure entry point to begin transacting on the blockchain in a decentralized and traceable manner.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

Just click "Execute" to use the method.

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "publicKey": "0x0ED99A476FCCeD2f609C80A312FDAFdeDEE85AA1"
}
```
{% endtab %}
{% endtabs %}
