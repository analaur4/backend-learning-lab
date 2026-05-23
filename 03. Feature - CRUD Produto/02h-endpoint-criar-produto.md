# História 02 — Criar produto

**Como** usuário da API,  
**quero** cadastrar um produto,  
**para** disponibilizá-lo para inclusão em pedidos.

## Endpoint sugerido

```http
POST /produtos
```

## Exemplo de request

```json
{
  "nome": "Teclado Mecânico",
  "descricao": "Teclado mecânico ABNT2",
  "preco": 250.00,
  "ativo": true
}
```

## Critérios de aceite

- Deve ser possível cadastrar um produto.
- O produto deve ser salvo no banco H2.
- A API deve retornar status `201 Created`.
- A resposta deve retornar os dados do produto criado.
