# História 01 — Criar a entidade Pedido

**Como** pessoa desenvolvedora iniciante,  
**quero** criar a entidade Pedido,  
**para** representar uma compra feita por um cliente.

## Atributos sugeridos

- `id`
- `cliente`
- `produtos`
- `dataCriacao`
- `status`
- `valorTotal`

## Relacionamentos sugeridos

- `Pedido` possui relação `@ManyToOne` com `Cliente`.
- `Pedido` possui relação `@ManyToMany` com `Produto`.

## Conceitos praticados

- Relacionamento `@ManyToOne`
- Relacionamento `@ManyToMany`
- Enum para status do pedido
- Cálculo de valor total
- Datas com `LocalDateTime`

## Critérios de aceite

- Deve existir uma entidade `Pedido` anotada com `@Entity`.
- O pedido deve estar relacionado a um cliente.
- O pedido deve estar relacionado a uma lista de produtos.
- As tabelas relacionadas devem ser criadas no H2.
