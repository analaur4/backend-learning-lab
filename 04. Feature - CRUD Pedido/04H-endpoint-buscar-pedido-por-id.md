# História 04 — Buscar pedido por ID

**Como** usuário da API,  
**quero** buscar um pedido específico pelo ID,  
**para** visualizar seus detalhes.

## Endpoint sugerido

```http
GET /pedidos/{id}
```

## Critérios de aceite

- Deve ser possível buscar um pedido por ID.
- Caso o pedido exista, deve retornar status `200 OK`.
- Caso o pedido não exista, deve retornar status `404 Not Found`.
- A resposta deve conter cliente, produtos, status, data e valor total.
