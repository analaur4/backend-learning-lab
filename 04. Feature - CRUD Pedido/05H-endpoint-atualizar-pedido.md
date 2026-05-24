# História 05 — Atualizar pedido

**Como** usuário da API,  
**quero** atualizar os produtos de um pedido,  
**para** corrigir ou alterar os itens comprados.

## Endpoint sugerido

```http
PATCH /pedidos/{id}
```

## Exemplo de request

```json
{
  "clienteId": 1,
  "produtosIds": [2, 4]
}
```

## Regras sugeridas

- O pedido deve existir.
- O cliente informado deve existir.
- Todos os produtos informados devem existir.
- O valor total deve ser recalculado.

## Critérios de aceite

- Deve ser possível atualizar um pedido existente.
- Caso o pedido não exista, deve retornar `404 Not Found`.
- Caso o cliente ou algum produto não exista, deve retornar `404 Not Found`.
- O valor total deve ser atualizado corretamente.
