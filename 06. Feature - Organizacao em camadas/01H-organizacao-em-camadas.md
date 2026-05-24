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
-  `mapper`: responsável por converter entidades em DTOs e DTOs em entidades.

## Critérios de aceite

- Controllers não devem acessar diretamente repositories.
- Services devem conter as regras de negócio.
- Repositories devem estender `JpaRepository`.
- DTOs devem ser usados nas entradas e saídas da API.
- Conversões entre DTO e Entity devem utilizar MapStruct.
- Services não devem conter lógica manual extensa de conversão de objetos.