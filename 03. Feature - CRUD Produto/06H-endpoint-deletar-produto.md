# História 06 — Deletar produto

**Como** usuário da API,  
**quero** remover um produto,  
**para** retirar produtos que não devem mais ser usados.

## Endpoint sugerido

```http
DELETE /produtos/{id}
```

## Critérios de aceite

- Deve ser possível deletar um produto pelo ID.
- Caso o produto exista, deve retornar status `204 No Content`.
- Caso o produto não exista, deve retornar status `404 Not Found`.
