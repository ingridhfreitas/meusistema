# 📦 Sistema de Fornecedores e Clientes

Este projeto é uma aplicação backend desenvolvida em **Java + Spring Boot** para gerenciamento de fornecedores (e futuramente clientes).  
A API segue arquitetura em camadas (Controller, Service, Repository, Model) e utiliza **JPA/Hibernate** para persistência em banco de dados.

---

## 🚀 Tecnologias utilizadas

- Java 17+  
- Spring Boot  
- Spring Data JPA (Hibernate)  
- Banco de Dados (H2/MySQL/PostgreSQL — configurável)  
- Lombok  
- Maven  

---

## 📂 Estrutura do projeto

api/
└── src/
└── main/
└── java/br/com/meusistema/api
├── controller/ -> Endpoints REST
├── service/ -> Regras de negócio
├── repository/ -> Persistência de dados
├── model/ -> Entidades (Fornecedor, Cliente, etc.)
└── enums/ -> Enumerações (ex: TipoFornecedorEnum)

### Fornecedores

| Método | Endpoint         | Descrição                         | Corpo (JSON)                                   |
|--------|------------------|-----------------------------------|-----------------------------------------------|
| POST   | `/fornecedores`  | Cria um novo fornecedor           | `{ "nomeFantasia": "...", "email": "...", "cnpj": "...", "tipoFornecedorEnum": "..." }` |

> ⚠️ Por enquanto apenas o **cadastro de fornecedores** está implementado (`POST /fornecedores`).  
As operações de listagem, atualização e exclusão podem ser adicionadas em breve.

---

## ▶️ Como executar o projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/ingridhfreitas/meusistema.git
Acesse o diretório da API:

bash
Copiar código
cd meusistema/api
Compile e rode a aplicação:

bash
Copiar código
mvn spring-boot:run
A aplicação estará disponível em:

arduino
Copiar código
http://localhost:8080
