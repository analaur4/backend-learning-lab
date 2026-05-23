# História 06 — Deletar cliente

**Como** usuário da API,  
**quero** remover um cliente,  
**para** excluir clientes que não devem mais estar cadastrados.

## Endpoint sugerido

```http
DELETE /clientes/{id}
```

## Critérios de aceite

- Deve ser possível deletar um cliente pelo ID.
- Caso o cliente exista, a API deve retornar status `204 No Content`.
- Caso o cliente não exista, a API deve retornar status `404 Not Found`.
