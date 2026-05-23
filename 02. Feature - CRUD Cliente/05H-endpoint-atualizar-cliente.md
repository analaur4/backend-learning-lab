# História 05 — Atualizar cliente

**Como** usuário da API,  
**quero** atualizar os dados de um cliente,  
**para** manter suas informações corretas no sistema.

## Endpoint sugerido

```http
PUT /clientes/{id}
```

## Critérios de aceite

- Deve ser possível atualizar os dados de um cliente existente.
- Caso o cliente exista, a API deve retornar status `200 OK`.
- Caso o cliente não exista, a API deve retornar status `404 Not Found`.
- Os dados atualizados devem ser persistidos no banco.
