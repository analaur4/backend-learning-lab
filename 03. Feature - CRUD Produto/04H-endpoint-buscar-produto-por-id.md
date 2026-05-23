# História 04 — Buscar produto por ID

**Como** usuário da API,  
**quero** buscar um produto específico pelo ID,  
**para** visualizar seus dados detalhados.

## Endpoint sugerido

```http
GET /produtos/{id}
```

## Critérios de aceite

- Deve ser possível buscar produto por ID.
- Caso o produto exista, deve retornar status `200 OK`.
- Caso o produto não exista, deve retornar status `404 Not Found`.
