# História 03 — Listar todos os produtos

**Como** usuário da API,  
**quero** listar todos os produtos cadastrados,  
**para** visualizar quais produtos estão disponíveis.

## Endpoint sugerido

```http
GET /produtos
```

## Critérios de aceite

- Deve ser possível listar todos os produtos.
- A API deve retornar status `200 OK`.
- A resposta deve ser uma lista de produtos.
- Caso não existam produtos, deve retornar uma lista vazia.
