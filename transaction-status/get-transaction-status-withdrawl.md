---
description: Check the status of a cryptocurrency withdrawal transaction by transaction ID
---

# \[GET] /transaction-status/withdrawl

O método **\[GET] /transaction-status/withdrawl** permite verificar o status de uma transação de saque de criptomoedas, utilizando o ID único da transação. Ao fornecer o ID, o método retorna o estado atual da retirada, informando se a transação foi processada, está em andamento ou se houve algum erro. Esse recurso é essencial para usuários que desejam acompanhar o progresso de seus saques, oferecendo uma visão clara e em tempo real sobre o status da transação e garantindo maior transparência e confiança nas operações financeiras.

### Authorization

Bearer token allows requests to be authenticated using an access key, such as a JSON Web Token (JWT). The token is a text string included in the request header.

```
Bearer <Your API token>
```

### Request Body

To check the status of a conversion transaction, simply enter the transaction ID and then click "Execute".

**Parameters**

<table><thead><tr><th width="364">Name</th><th>Description</th></tr></thead><tbody><tr><td>transactionId</td><td>Conversion transaction ID to check status</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "transactionId": "TX987654",
  "status": "Pending"
}
```
{% endtab %}
{% endtabs %}
