# História 02 — Criar pedido

**Como** usuário da API,  
**quero** criar um pedido informando cliente e produtos,  
**para** registrar uma compra no sistema.

## Endpoint sugerido

```http
POST /pedidos
```

## Exemplo de request

```json
{
  "clienteId": 1,
  "produtosIds": [1, 2, 3]
}
```

## Regras sugeridas

- O cliente informado deve existir.
- Todos os produtos informados devem existir.
- O pedido deve calcular o valor total com base nos produtos.
- A data de criação deve ser preenchida automaticamente.
- O status inicial pode ser `CRIADO`.

## Critérios de aceite

- Deve ser possível criar um pedido válido.
- Caso o cliente não exista, deve retornar `404 Not Found`.
- Caso algum produto não exista, deve retornar `404 Not Found`.
- O valor total deve ser calculado corretamente.
- A API deve retornar status `201 Created`.
