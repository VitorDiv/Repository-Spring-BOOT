# 📌 Spring Boot + Data JPA (Exemplo Simples)

Projeto de exemplo utilizando **Spring Boot** com **Spring Data JPA** e banco em memória **H2**, com o objetivo de demonstrar operações básicas de persistência de dados.

---

## 🚀 Tecnologias utilizadas

* Java 17
* Spring Boot
* Spring Data JPA
* H2 Database
* Maven

---

## 📂 Estrutura do Projeto

* `entity` → Classe que representa a tabela no banco (`User`)
* `repository` → Interface de acesso aos dados (`UserRepository`)
* Classe principal → Inicializa a aplicação e executa testes

---

## 🧠 Funcionamento

Ao iniciar a aplicação:

1. Dois usuários são inseridos automaticamente no banco:

   * João
   * Maria

2. Todos os usuários são buscados e exibidos no console.

---

## 🗄️ Entidade

A aplicação possui uma entidade simples:

* **User**

  * `id` (Long) → chave primária
  * `name` (String)

---

## 🔄 Operações com JPA

O projeto utiliza o `JpaRepository`, que já fornece métodos prontos como:

* `save()` → salvar dados
* `findAll()` → listar todos os registros

---

## ▶️ Como executar

1. Clone o projeto:

```bash
git clone <url-do-repositorio>
```

2. Acesse a pasta:

```bash
cd demo
```

3. Execute:

```bash
./mvnw spring-boot:run
```

---

## 🌐 Acesso ao banco H2

Após iniciar a aplicação, acesse:

```
http://localhost:8080/h2-console
```

### Configuração padrão:

* JDBC URL: `jdbc:h2:mem:testdb`
* User: `sa`
* Password: (deixe vazio)

---

## 📌 Observações

* O banco H2 é **em memória**, ou seja, os dados são apagados ao parar a aplicação.
* Este projeto é apenas para fins de estudo e aprendizado de JPA.

---

## ✍️ Autor

Projeto desenvolvido para prática com Spring Boot e persistência de dados.
