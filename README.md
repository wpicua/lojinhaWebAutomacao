# Lojinha Web Automação

Esse é um repositório que contem a automação de alguns testes em Web de um software denominado Lojinha. Os sub-tópicos abaixo descrevem algumas decisões na estrutura do projeto.

## Tecnologias Utuilizadas

- Java
  https://www.oracle.com/java/technologies/downloads/#jdk18-windows
- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine/5.9.0
- RestAssured
  https://mvnrepository.com/artifact/io.rest-assured/rest-assured/5.1.1
- Maven
  https://maven.apache.org/

## Testes Automatizados

- Testes para validar as partições de equivalência relacionadas ao valor do produto a lojinha, que estão vinculados diretamente a regra de negocio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais

- Sempre utilizamos um método que captura o nome de usuário e a senha, e posteriormente também temos um método que submete o formulário de login.
- Acessamos o formulário de adição de produto, onde adicionamos o nome, o valor e a cor do produto, e submetemos o formulário com erro ou com sucesso.
- Nesse projeto fazemos uso do JUnit 5, o que nos da a possibilidade de usar a anotação DisplayName para dar descrições em Português para nossos testes.