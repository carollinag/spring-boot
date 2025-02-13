# Spring Boot API RESTful

### Este projeto é uma API RESTful desenvolvida com Spring Boot, implementando os níveis de maturidade do modelo Richardson (RMM). Ele demonstra boas práticas no desenvolvimento de APIs REST e utiliza diversas dependências do ecossistema Spring.

## Modelo de Maturidade de Richardson

A API foi projetada para atender aos diferentes níveis do modelo de maturidade de Richardson:

| Nível | Características                                    |
|-------|----------------------------------------------------|
|0| API funciona como um único endpoint (RPC).         |
|1| Uso de recursos, mas sem verbos HTTP corretamente. |
|2| Uso correto dos verbos HTTP e códigos de status.|
|3| HATEOAS – API fornece links de navegação.|

### Tecnologias Utilizadas

O projeto foi desenvolvido utilizando as seguintes tecnologias:

* Java 17

* Spring Boot 3.4.2

* Maven para gerenciamento de dependências

* Spring Data JPA para interação com banco de dados

* Spring Validation para validação de dados

* Spring Web para construção da API REST

* Spring HATEOAS para implementação do nível 3 do modelo RMM

* Banco de dados H2 (banco em memória para testes)

* Spring Boot DevTools para facilitar o desenvolvimento

* SpringDoc OpenAPI para documentação da API

### Como Executar o Projeto

1. Clone este repositório:
 ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
 ```

2. Acesse o diretório do projeto:
 ```
cd nome-do-projeto
 ```
3. Compile e execute o projeto com Maven:
 ```bash
mvn spring-boot:run
 ```
4. Acesse o console do H2:
 ```
http://localhost:8080/h2-console
 ```
Para testar a API, utilize ferramentas como Postman para fazer chamadas aos endpoints disponíveis:
 ```
- Listar todos os produtos: GET http://localhost:8080/products
- Buscar um produto por ID: GET http://localhost:8080/products/{id}
- Criar um novo produto: POST http://localhost:8080/products
- Atualizar um produto: PUT http://localhost:8080/products/{id}
- Deletar um produto: DELETE http://localhost:8080/products/{id}
 ```
