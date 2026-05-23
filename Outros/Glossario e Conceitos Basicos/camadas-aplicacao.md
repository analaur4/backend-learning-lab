# Glossário e conceitos - Camadas de uma aplicação

## O que é uma Entidade (`@Entity`)?

Uma entidade representa uma tabela do banco de dados.

Exemplo:

```java id="pl0ch7"
@Entity
public class Produto {
}
```

---

## O que é Repository?

O Repository é a camada responsável por acessar o banco de dados.

Exemplo:

```java id="r5q2pd"
public interface ClienteRepository
        extends JpaRepository<Cliente, Long> {
}
```

---

## O que é Service?

A camada Service contém as regras de negócio da aplicação.

Ela fica entre:

* Controller
* Repository

---

## O que é Controller?

O Controller expõe os endpoints da API.

Exemplo:

```java id="nhm6ee"
@RestController
@RequestMapping("/clientes")
public class ClienteController {
}
```

---

## O que é DTO?

DTO significa:

```text id="wnof0m"
Data Transfer Object
```

É um objeto utilizado para transferência de dados entre camadas.

Objetivo:

* evitar expor entidades diretamente
* controlar entrada e saída da API

---

## O que são validações?

Validações garantem que os dados recebidos sejam válidos.

Exemplo:

```java id="stwl2d"
@NotBlank
private String nome;
```