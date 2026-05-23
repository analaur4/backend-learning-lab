# História 01 — Criar o projeto Spring Boot

**Como** pessoa desenvolvedora iniciante,  
**quero** criar um projeto Spring Boot do zero,  
**para** entender a estrutura inicial de uma aplicação backend Java.

## Descrição

Criar o projeto utilizando o [**Spring Initializr**](https://start.spring.io/), configurando as dependências iniciais necessárias para o desenvolvimento da API.

## Configurações sugeridas

- Project: Maven
- Language: Java
- Spring Boot: versão estável mais recente
- Java: 21
- Packaging: Jar
- Group: `br.com`
- Artifact: `pedidos-api`

## Dependências iniciais

- Spring Web
- Spring Data JPA
- H2 Database
- Lombok
- Validation

## Critérios de aceite

- O projeto deve ser criado com sucesso pelo Spring Initializr.
- A aplicação deve executar sem erros.
- Deve existir uma classe principal com `@SpringBootApplication`.
- Ao iniciar a aplicação, o Spring Boot deve subir corretamente.
