API - Spring Boot

API REST feita com Spring Boot para gerenciar usuários na memória, sem usar banco de dados. Os dados ficam guardados num Map<Long, User>. Tem as operações básicas: criar, listar, atualizar e apagar usuário.

Funcionalidades

Criar usuário (POST /users)

Listar usuários (GET /users)

Atualizar usuário por Id (PUT /users/{id})

Apagar usuário por Id (DELETE /users/{id})

Como executar

Tenha o Java 17+ e o Maven instalados na sua máquina.

Clone este repositório:
git clone https://github.com/paulobaisch1/api-rest-PB

Entre na pasta do projeto e rode:
mvn clean spring-boot:run

A API vai rodar no endereço http://localhost:8080

Estrutura do projeto

src
├── main
│ ├── java
│ │ └── com.example.atvAPI
│ │ ├── model
│ │ │ └── User.java
│ │ ├── service
│ │ │ └── UserService.java
│ │ ├── controller
│ │ │ └── UserController.java
│ │ └── AtvApiApplication.java
│ └── resources
│ └── application.properties

Testes com Postman

Os endpoints foram testados no Postman para garantir que funcionam bem. Exemplos:

Criar usuário
POST /users
{ "nome": "Gustavo", "idade": 20 }

Listar usuários
GET /users

Atualizar usuário
PUT /users/1
{ "nome": "Paulo", "idade": 20 }

Apagar usuário
DELETE /users/1

Tecnologias usadas

Java

Spring Boot

Maven

Postman
