# História 04 — Buscar cliente por ID

**Como** usuário da API,  
**quero** buscar um cliente específico pelo ID,  
**para** visualizar seus dados detalhados.

## Endpoint sugerido

```http
GET /clientes/{id}
```

## Critérios de aceite

- Deve ser possível buscar um cliente pelo ID.
- Caso o cliente exista, a API deve retornar status `200 OK`.
- Caso o cliente não exista, a API deve retornar status `404 Not Found`.
