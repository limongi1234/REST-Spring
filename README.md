# REST-Spring — API REST com Spring Boot 🌱

> 🔱 **Fork** de um projeto da [DIO](https://www.dio.me), originalmente criado por **Kaique Arantes Costa**. Repositório mantido aqui para **estudo e referência** — o código pertence ao autor original.

API REST construída com **Spring Boot**, demonstrando uma aplicação completa com **autenticação JWT**, controle de acesso por perfis (roles), CRUD de produtos e pedidos, tratamento de exceções e monitoramento.

## ✨ Funcionalidades

- **Autenticação e autorização** com **JWT** (login e proteção de rotas)
- **Usuários e perfis** (`User`, `Role`) com Spring Security
- **CRUD** de **Produtos** e **Pedidos**
- **Tratamento de exceções** centralizado (`@ControllerAdvice`, exceções customizadas)
- **Health check** e monitoramento via **Spring Boot Actuator** + **Spring Boot Admin**

## 🧩 Organização

```
config/      → segurança (SecurityConfig) e JWT (filter, token util, entry point)
auth/        → entidades, repositórios, serviços e controller de autenticação
entity/      → Produto e Pedido
repository/  → repositórios JPA
service/     → regras de negócio
controller/  → endpoints REST + ControllerAdvice
exception/   → exceções customizadas
```

## 🛠️ Tecnologias

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat&logo=springsecurity&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)
![H2](https://img.shields.io/badge/H2_Database-09476B?style=flat&logo=h2&logoColor=white)

- **Java + Spring Boot** (Web, Data JPA, Security, Actuator)
- **JWT** (jjwt) — autenticação stateless
- **H2** — banco em memória
- **Spring Boot Admin** — monitoramento

## 🚀 Como executar

```bash
git clone https://github.com/limongi1234/REST-Spring.git
cd REST-Spring

./mvnw spring-boot:run
```

A aplicação sobe em `http://localhost:8080`. O console do H2 e o Actuator ficam disponíveis nas rotas padrão do Spring.

> 📚 Material de estudo sobre APIs REST com Spring Boot, Security e JWT.
