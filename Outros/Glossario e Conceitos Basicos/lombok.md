# Conceitos sobre Lombok

## O que é Lombok?

Project Lombok é uma biblioteca que reduz código repetitivo.

Ela gera automaticamente:

* getters
* setters
* construtores
* equals/hashCode
* toString

---

## Exemplo sem Lombok

```java id="q59qdr"
public class Cliente {

    private String nome;

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }
}
```

---

## Exemplo com Lombok

```java id="jlwm5v"
@Getter
@Setter
public class Cliente {
    private String nome;
}
```
