# API de Biblioteca - Spring Boot

Projeto desenvolvido como parte do aprendizado de **Spring Boot 3** e **Java 17**. Este projeto é uma API RESTful para gerenciar livros e autores, utilizando **Spring Data JPA** e **H2 Database**.

## 🛠 Funcionalidades Implementadas

- **Cadastro e listagem de livros e autores**
- **Documentação da API** gerada automaticamente via **Swagger**
- **Persistência de dados** utilizando **Spring Data JPA** e **H2 Database** (em memória)

## 🔥 Tecnologias Utilizadas

- Java 17
- Spring Boot 3
- Spring Data JPA
- H2 Database (em memória)
- Swagger (Documentação da API)
- Maven
- IntelliJ IDEA (IDE utilizada)

## 📚 Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/rafafdx/biblioteca-api.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd biblioteca-api
   ```
3. Abra o projeto na sua IDE de preferência (como IntelliJ IDEA ou Eclipse).

4. Rode a aplicação (classe ```BibliotecaApplication```).

5. Acesse a API e a documentação no navegador:

- Swagger UI: http://localhost:8080/swagger-ui.html  
- Console do H2: http://localhost:8080/h2-console  
- URL do banco: `jdbc:h2:mem:biblioteca-db`  
- Usuário: `sa`  
- Senha: (deixe em branco)

## ✅ Exemplos de Endpoints

GET /autores - Lista todos os autores

POST /autores - Cria um novo autor

Exemplo de corpo da requisição:
```
  {
    "nome": "Machado de Assis"
  }
```
GET /livros - Lista todos os livros

POST /livros - Cria um novo livro

Exemplo de corpo da requisição:
```
  {
    "titulo": "Dom Casmurro",
    "autor": {
      "id": 1
    }
  }
```

Feito com 💻 por rafafdx
