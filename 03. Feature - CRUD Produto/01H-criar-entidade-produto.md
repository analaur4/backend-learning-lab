# História 01 — Criar a entidade Produto

**Como** pessoa desenvolvedora iniciante,  
**quero** criar a entidade Produto,  
**para** representar os itens que poderão ser incluídos em pedidos.

## Atributos sugeridos

- `id`
- `nome`
- `descricao`
- `preco`
- `ativo`

## Conceitos praticados

- Entidade JPA
- Tipos numéricos com `BigDecimal`
- Validação de valores monetários
- Boas práticas para valores financeiros

## Critérios de aceite

- Deve existir uma classe `Produto` anotada com `@Entity`.
- O produto deve possuir um identificador único.
- O preço deve ser representado com `BigDecimal`.
- A tabela de produtos deve ser criada no H2.
