# Backlog Didático — API de Pedidos com Java 21 e Spring Boot

## Visão geral do projeto

Criar uma API REST simples para registro de pedidos, com foco em consolidar conceitos básicos de desenvolvimento backend usando Java 21, Spring Boot, Maven, H2, Lombok, Bean Validation e JPA.

A aplicação terá três entidades principais:

- **Cliente**: pode possuir vários pedidos.
- **Produto**: pode estar presente em vários pedidos.
- **Pedido**: pertence a um único cliente e pode conter vários produtos.

Relacionamentos esperados:

- Um **Cliente** pode ter muitos **Pedidos**.
- Um **Pedido** pertence a apenas um **Cliente**.
- Um **Pedido** pode possuir muitos **Produtos**.
- Um **Produto** pode estar em muitos **Pedidos**.

---

# Conceitos trabalhados ao longo do projeto

- Criação de projeto Spring Boot
- Maven
- Java 21
- API REST
- Controllers
- Services
- Repositories
- DTOs
- JPA/Hibernate
- Banco H2
- Relacionamentos entre entidades
- Bean Validation
- Tratamento global de exceções
- Status HTTP
- Boas práticas básicas de organização backend
- Testes manuais de API
- Documentação inicial de projeto
