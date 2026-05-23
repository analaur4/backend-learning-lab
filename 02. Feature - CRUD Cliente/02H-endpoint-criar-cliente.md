# História 02 — Criar cliente

**Como** usuário da API,  
**quero** cadastrar um cliente,  
**para** permitir que ele realize pedidos futuramente.

## Endpoint sugerido

```http
POST /clientes
```

## Exemplo de request

```json
{
  "nome": "Ana Laura",
  "email": "ana@email.com",
  "telefone": "11999999999",
  "cpf": "12345678900"
}
```

## Critérios de aceite

- Deve ser possível cadastrar um cliente.
- O cliente deve ser salvo no banco H2.
- A API deve retornar status `201 Created`.
- A resposta deve retornar os dados do cliente criado.
