# História 01 — Criar tratamento global de exceções

**Como** pessoa desenvolvedora,  
**quero** centralizar o tratamento de erros da API,  
**para** padronizar as respostas de erro.

## Descrição

Criar uma classe com `@RestControllerAdvice` para tratar erros comuns da aplicação.

## Erros sugeridos

- Registro não encontrado
- Erro de validação de request
- Erro inesperado

## Conceitos praticados

- `@RestControllerAdvice`
- `@ExceptionHandler`
- Respostas HTTP padronizadas
- Criação de DTO de erro

## Critérios de aceite

- A API deve retornar erros padronizados.
- Erros de validação devem retornar `400 Bad Request`.
- A resposta deve indicar os campos inválidos.
- Registros não encontrados devem retornar `404 Not Found`.
- Erros inesperados devem retornar `500 Internal Server Error`.
