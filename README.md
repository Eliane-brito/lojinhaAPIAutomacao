# 🔗 Lojinha API - Projeto de Automação de Testes

Este repositório contém a automação de testes para a API REST da aplicação **Lojinha**. O objetivo é garantir a validação de regras de negócio e comportamentos esperados da API, utilizando boas práticas de organização e escrita de testes automatizados.

---

## 🚀 Tecnologias Utilizadas

- [Java](https://www.oracle.com/ae/java/technologies/downloads/)
- [JUnit 5](https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.7.1)
- [RestAssured](https://mvnrepository.com/artifact/io.rest-assured/rest-assured/5.5.1)
- [Maven](https://maven.apache.org/)

---

## ✅ Testes Automatizados

Foram implementados testes para validar as **partições de equivalência** relacionadas à regra de negócio da Lojinha:

> O valor do produto deve estar entre **R$ 0,01 e R$ 7.000,00**.

Os testes cobrem diferentes cenários, garantindo que a API aceite apenas valores dentro do intervalo permitido e rejeite valores inválidos com as mensagens de erro apropriadas.

---

## 🛠️ Boas Práticas e Arquitetura

- Utilização da anotação `@BeforeEach` para capturar o **token de autenticação**, reutilizado nos testes subsequentes.
- Armazenamento dos dados enviados à API por meio de classes **POJO**, garantindo organização e clareza nos dados manipulados.
- Criação de dados dinâmicos com a **classe Data Factory**, facilitando a geração e controle de dados para diferentes cenários.
- Uso da anotação `@DisplayName` do **JUnit 5** para descrever os testes em **português**, melhorando a legibilidade e documentação dos testes.

---

## 💡 Considerações Finais

Este projeto tem como finalidade a prática e demonstração de conhecimentos em automação de testes de API REST com Java. Ele pode ser expandido com mais cenários, integrações e validações conforme a evolução da aplicação Lojinha.

---
o JUnit 5, o que nos dá a possibilidade de usar a anotação  DislayName para dar descrições em Português para nossos testes.