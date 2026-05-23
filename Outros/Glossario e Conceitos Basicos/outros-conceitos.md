# Outros conceitos

# O que é Injeção de Dependência?

Dependency Injection é um padrão utilizado pelo Spring para fornecer objetos automaticamente.

Exemplo:

```java id="vg4k7c"
@RequiredArgsConstructor
public class ClienteService {

    private final ClienteRepository repository;
}
```

O Spring cria e injeta o objeto automaticamente.

---

# O que é uma anotação?

Anotações são metadados utilizados para configurar comportamentos.

Exemplos:

* `@Entity`
* `@Service`
* `@RestController`
* `@Autowired`

---

# O que é o Spring Initializr?

[Spring Initializr](https://start.spring.io?utm_source=chatgpt.com)

Ferramenta utilizada para gerar projetos Spring Boot prontos.

Ela permite escolher:

* Java version
* Maven/Gradle
* Dependências
* Versão do Spring Boot

---

# Estrutura comum de um projeto Spring Boot

```text id="0j4g5u"
src/main/java
 ├── controller
 ├── service
 ├── repository
 ├── entity
 ├── dto
 └── exception
```

---

# O que é o `application.properties`?

Arquivo de configuração da aplicação.

Exemplo:

```properties id="zt8vkr"
server.port=8080
spring.datasource.url=jdbc:h2:mem:testdb
```

---

# O que é o Swagger/OpenAPI?

OpenAPI é uma ferramenta para documentação de APIs REST.

Permite:

* visualizar endpoints
* testar requisições
* documentar contratos
