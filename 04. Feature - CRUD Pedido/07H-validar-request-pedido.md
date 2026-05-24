# História 07 — Validar request de Pedido

**Como** pessoa desenvolvedora,  
**quero** validar os dados enviados na criação e atualização de pedidos,  
**para** evitar pedidos inválidos.

## Validações sugeridas

- `clienteId`: obrigatório
- `produtosIds`: obrigatório
- `produtosIds`: não pode ser uma lista vazia

## Conceitos praticados

- DTO de request
- Bean Validation
- `@NotNull`
- `@NotEmpty`
- Validação de listas
- Tratamento de erro padronizado

## Critérios de aceite

- Requests inválidas devem retornar status `400 Bad Request`.
- Pedidos inválidos não devem ser persistidos.
