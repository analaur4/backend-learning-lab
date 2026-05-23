# História 03 — Listar todos os clientes

**Como** usuário da API,  
**quero** listar todos os clientes cadastrados,  
**para** visualizar os clientes disponíveis no sistema.

## Endpoint sugerido

```http
GET /clientes
```

## Critérios de aceite

- Deve ser possível listar todos os clientes.
- A API deve retornar status `200 OK`.
- A resposta deve ser uma lista de clientes.
- Caso não existam clientes, a API deve retornar uma lista vazia.
