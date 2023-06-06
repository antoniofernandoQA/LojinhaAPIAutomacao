# Lojinha API Automação
Esse é um  repositório que contém a automação de alguns testes de API Rest de um software denominado Lojinha. Os sub tópicos abaixo descrevem algumas decisões tomadas na estruturação do projeto.

## Tecnologias Utilizadas
- Java
  https://www.oracle.com/br/java/technologies/downloads/
- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.10.0-M1
- Rest Assured
  https://mvnrepository.com/artifact/io.rest-assured/rest-assured/5.3.0
- Mavem
  https://maven.apache.org/

## Testes Automatizados
Testes para validar as partições de equivalência relacionadas ao valor do produto na Lojinha, que estão vinculados diretamente à regra de negócio que diz que o valor do produto deve estar entre 0,01 e 7.000,00 reais.

## Notas Gerais
- Sempre utilizamos a anotação BeforeEach para capturar o token que será utilizado posteriormente nos métodos de teste.
- Armazenamos os dados que são enviados para a API através do uso de classes pojo.
- Criamos dados iniciais através do uso de classe DataFactory, para facilitar a criação e controle dos mesmos.
- Nesse projeto fazemos uso do JUnit 5, o que nos dá a possibilidade de usar a anotação DisplayName para dar descrições em português para nossos testes.