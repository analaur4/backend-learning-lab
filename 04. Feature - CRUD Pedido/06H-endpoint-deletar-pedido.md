# História 06 — Deletar pedido

**Como** usuário da API,  
**quero** deletar um pedido,  
**para** remover registros que não devem mais existir.

## Endpoint sugerido

```http
DELETE /pedidos/{id}
```

## Critérios de aceite

- Deve ser possível deletar um pedido pelo ID.
- Caso o pedido exista, deve retornar status `204 No Content`.
- Caso o pedido não exista, deve retornar status `404 Not Found`.
