# História 07 — Validar request de Produto

**Como** pessoa desenvolvedora,  
**quero** validar os dados enviados na criação e atualização de produtos,  
**para** evitar cadastro de produtos inválidos.

## Validações sugeridas

- `nome`: obrigatório
- `preco`: obrigatório e maior que zero
- `descricao`: opcional
- `ativo`: obrigatório ou com valor padrão `true`

## Conceitos praticados

- DTO de request
- Bean Validation
- `@NotBlank`
- `@NotNull`
- `@DecimalMin`
- Tratamento de erro de validação

## Critérios de aceite

- Requests inválidas devem retornar status `400 Bad Request`.
- A resposta deve indicar os campos inválidos.
- Produtos inválidos não devem ser persistidos.
