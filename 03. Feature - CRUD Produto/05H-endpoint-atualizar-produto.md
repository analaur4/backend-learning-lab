# História 05 — Atualizar produto

**Como** usuário da API,  
**quero** atualizar os dados de um produto,  
**para** corrigir ou alterar informações cadastradas.

## Endpoint sugerido

```http
PUT /produtos/{id}
```

## Critérios de aceite

- Deve ser possível atualizar um produto existente.
- Caso o produto exista, deve retornar status `200 OK`.
- Caso o produto não exista, deve retornar status `404 Not Found`.
- Os dados atualizados devem ser persistidos no banco.
