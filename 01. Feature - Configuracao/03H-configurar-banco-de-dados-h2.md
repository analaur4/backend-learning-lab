# História 03 — Configurar o banco de dados H2

**Como** pessoa desenvolvedora iniciante,  
**quero** usar um banco de dados simples em memória,  
**para** praticar persistência de dados sem instalar um banco externo.

## Descrição

Configurar o banco de dados **H2** para ser usado durante o desenvolvimento da API.

## Explicação breve

O **H2** é um banco de dados relacional leve, que pode rodar em memória. Isso significa que os dados podem ser perdidos ao reiniciar a aplicação, mas ele é ótimo para aprendizado, testes e protótipos.

## Configuração sugerida no `application.properties`

```properties
spring.datasource.url=jdbc:h2:mem:pedidosdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=

spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.jpa.hibernate.ddl-auto=create
spring.jpa.show-sql=true

spring.h2.console.enabled=true
spring.h2.console.path=/h2-console
```

## Critérios de aceite

- A aplicação deve subir usando o banco H2.
- O console do H2 deve estar acessível em `/h2-console`.
- As tabelas devem ser criadas automaticamente pelo JPA/Hibernate.
- As queries SQL devem aparecer no console da aplicação.
