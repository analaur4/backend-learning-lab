# História 01 — Criar a entidade Cliente

**Como** pessoa desenvolvedora iniciante,  
**quero** criar a entidade Cliente,  
**para** representar os clientes que realizarão pedidos na API.

## Descrição

Criar a entidade `Cliente` utilizando JPA.

## Atributos sugeridos

A escolha final dos atributos fica a critério da pessoa desenvolvedora, mas uma sugestão seria:

- `id`
- `nome`
- `email`
- `telefone`
- `cpf`

## Conceitos praticados

- Entidade JPA
- `@Entity`
- `@Id`
- `@GeneratedValue`
- Mapeamento de colunas
- Lombok em entidades

## Critérios de aceite

- Deve existir uma classe `Cliente` anotada com `@Entity`.
- Deve existir um campo identificador `id`.
- O `id` deve ser gerado automaticamente.
- A tabela de clientes deve ser criada no H2.
