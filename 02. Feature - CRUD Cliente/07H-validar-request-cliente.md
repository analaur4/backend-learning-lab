# História 07 — Validar request de Cliente

**Como** pessoa desenvolvedora,  
**quero** validar os dados enviados na criação e atualização de clientes,  
**para** evitar o cadastro de informações inválidas.

## Validações sugeridas

- `nome`: obrigatório
- `email`: obrigatório e com formato válido
- `cpf`: obrigatório
- `telefone`: opcional ou obrigatório, a critério do grupo

## Conceitos praticados

- DTO de request
- Bean Validation
- `@Valid`
- `@NotBlank`
- `@Email`
- Tratamento de erro de validação

## Critérios de aceite

- Requests inválidas devem retornar status `400 Bad Request`.
- A entidade não deve ser salva caso a request seja inválida.
