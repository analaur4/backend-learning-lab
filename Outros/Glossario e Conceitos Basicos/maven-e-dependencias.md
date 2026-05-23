# Conceitos sobre Maven

## O que é Maven?

Apache Maven é uma ferramenta de gerenciamento de dependências e build de projetos Java.

Ele é responsável por:

* baixar bibliotecas automaticamente
* compilar o projeto
* executar testes
* gerar artefatos (`.jar`)
* organizar o ciclo de build

---

## O que é dependência?

Dependências são bibliotecas externas utilizadas no projeto.

Exemplo:

* Spring Boot
* Lombok
* Hibernate
* JUnit

No Maven, elas ficam no arquivo:

```xml id="vdujlwm"
pom.xml
```

---

## Maven vs Gradle

| Maven                        | Gradle                 |
| ---------------------------- | ---------------------- |
| Mais tradicional             | Mais moderno           |
| XML                          | DSL mais flexível      |
| Mais simples para iniciantes | Mais customizável      |
| Muito usado em empresas Java | Muito usado em Android |
