# 🛠️ Projeto Web Services com Spring Boot, JPA e Hibernate

Este repositório contém um sistema de pedidos desenvolvido com **Spring Boot**, utilizando **JPA/Hibernate** para persistência, e **PostgreSQL**/**H2** como banco de dados. O projeto foi inspirado em um curso completo de desenvolvimento de web services RESTful com Java, cobrindo desde as entidades básicas até o deploy na nuvem com Heroku.

## 📚 Tecnologias Utilizadas

- **Java 17+**
- **Spring Boot**
- **Spring Data JPA**
- **Hibernate**
- **Banco H2 (testes)** e **PostgreSQL (produção)**
- **Maven**
- **Heroku CLI**
- **Postman** (para testes)
- **Lombok**

## 📦 Funcionalidades

- ✅ CRUD completo para entidade `User`
- ✅ Mapeamento de entidades:
  - `User`, `Order`, `Product`, `Category`, `OrderItem`, `Payment`
- ✅ Relacionamentos:
  - OneToMany, ManyToMany, OneToOne com JoinTable e dados extras
- ✅ Enum customizado: `OrderStatus`
- ✅ Cálculo de subtotal e total de pedidos
- ✅ Tratamento de exceções com respostas padronizadas
- ✅ Perfis de ambiente: `test`, `dev`, `prod`
- ✅ Deploy na nuvem com Heroku
- ✅ Execução de script SQL em ambiente remoto

## 🗂️ Organização do Projeto

```bash
src
├── main
│   ├── java
│   │   └── com.example.project
│   │       ├── entities
│   │       ├── repositories
│   │       ├── resources
│   │       ├── services
│   │       └── config
│   └── resources
│       ├── application.properties
│       └── static / templates (se houver)
├── test
│   └── com.example.project
└── pom.xml
