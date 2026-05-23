# Conceitos sobre tratamento de erros

## O que é tratamento global de erros?

É uma forma centralizada de tratar exceções da aplicação.

Objetivo:

* padronizar respostas de erro
* evitar duplicação
* melhorar legibilidade

---

## O que é Exception Handler?

Um Exception Handler intercepta erros lançados pela aplicação.

Exemplo:

```java id="l4zmbi"
@ExceptionHandler(EntityNotFoundException.class)
```

---

## O que é `@ControllerAdvice`?

`@ControllerAdvice` é uma anotação do Spring Boot usada para criar handlers globais.

Exemplo:

```java id="nsmhtf"
@ControllerAdvice
public class GlobalExceptionHandler {
}
```

---

## Exemplo de fluxo de erro

```text id="n8d0jv"
Controller
↓
Service
↓
Erro lançado
↓
Handler captura erro
↓
Resposta padronizada
```

---

## Exemplo de resposta de erro

```json id="u88m1y"
{
  "message": "Cliente não encontrado",
  "status": 404
}
```
