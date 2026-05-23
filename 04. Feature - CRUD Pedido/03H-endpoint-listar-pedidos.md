# História 03 — Listar todos os pedidos

**Como** usuário da API,  
**quero** listar todos os pedidos,  
**para** visualizar os pedidos registrados no sistema.

## Endpoint sugerido

```http
GET /pedidos
```

## Critérios de aceite

- Deve ser possível listar todos os pedidos.
- A API deve retornar status `200 OK`.
- A resposta deve conter os dados do pedido, cliente e produtos.
- Caso não existam pedidos, deve retornar uma lista vazia.
