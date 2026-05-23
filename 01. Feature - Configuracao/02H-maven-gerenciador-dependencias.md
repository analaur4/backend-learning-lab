# História 02 — Configurar o Maven como gerenciador de dependências

**Como** pessoa desenvolvedora iniciante,  
**quero** entender o papel do Maven no projeto,  
**para** saber como as dependências são gerenciadas em uma aplicação Java.

## Descrição

Utilizar o Maven como gerenciador de dependências e ferramenta de build do projeto.

## Explicação breve

O **Maven** é uma ferramenta que gerencia dependências, build, empacotamento e execução de testes em projetos Java. Ele utiliza o arquivo `pom.xml` para declarar bibliotecas, plugins e configurações do projeto.

## Comparativo breve com Gradle

- **Maven**: mais declarativo, usa XML, muito comum em projetos corporativos Java.
- **Gradle**: mais flexível, usa Groovy ou Kotlin, costuma ser mais customizável.

Para este projeto, o Maven será usado por ser simples, bastante difundido e adequado para aprendizado inicial.

## Critérios de aceite

- O projeto deve possuir um arquivo `pom.xml`.
- As dependências devem estar declaradas no `pom.xml`.
- O projeto deve compilar usando Maven.
- O comando `mvn clean install` deve executar com sucesso.
