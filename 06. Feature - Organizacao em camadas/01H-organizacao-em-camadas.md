# História 01 — Separar Controller, Service e Repository

**Como** pessoa desenvolvedora iniciante,  
**quero** organizar o projeto em camadas,  
**para** entender melhor a responsabilidade de cada parte da aplicação.

## Descrição

Separar o código da aplicação nas camadas principais:

- `controller`: recebe as requisições HTTP.
- `service`: concentra regras de negócio.
- `repository`: acessa o banco de dados.
- `entity`: representa as tabelas do banco.
- `dto`: representa os dados de entrada e saída da API.

## Critérios de aceite

- Controllers não devem acessar diretamente repositories.
- Services devem conter as regras de negócio.
- Repositories devem estender `JpaRepository`.
- DTOs devem ser usados nas entradas e saídas da API.
