# Glossário e conceitos - Hibernate, ORM, JPA, H2

## O que é Hibernate?

Hibernate é um framework ORM (Object Relational Mapping).

Ele faz o mapeamento entre:

* objetos Java
* tabelas do banco de dados

---

### Exemplo

Classe Java:

```java id="28tr1t"
@Entity
public class Cliente {
}
```

Tabela gerada:

```sql id="4i8o7n"
CREATE TABLE cliente
```

---

## O que é ORM?

ORM significa:

```text id="b7n9zv"
Object Relational Mapping
```

Ou seja:

* objetos viram tabelas
* atributos viram colunas

---

## O que é JPA?

Jakarta Persistence API é uma especificação Java para persistência de dados.

O Hibernate é a implementação mais famosa da JPA.

---

### Relação entre JPA e Hibernate

| Tecnologia | Papel         |
| ---------- | ------------- |
| JPA        | Especificação |
| Hibernate  | Implementação |

---

## O que é H2 Database?

H2 Database é um banco de dados leve muito utilizado em estudos e testes.

---

### Principais características

* Fácil configuração
* Rápido
* Pode rodar em memória
* Não precisa instalar servidor
* Muito usado em desenvolvimento local

---

## H2 em Memória

Exemplo:

```properties id="4owr12"
spring.datasource.url=jdbc:h2:mem:testdb
```

Nesse modo:

* o banco existe apenas enquanto a aplicação estiver rodando
* ao desligar a aplicação, os dados são perdidos

---

## H2 Persistente em Arquivo

Exemplo:

```properties id="t2v5uh"
spring.datasource.url=jdbc:h2:file:./data/testdb
```

Nesse modo:

* os dados ficam salvos em disco
* continuam após reiniciar a aplicação
