# Literalura 🚀

Aplicação de console em Java + Spring Boot para gerenciar uma biblioteca, consumindo dados da API Gutendex e armazenando-os em PostgreSQL.

## 🔍 Funcionalidades

* Buscar livros por título via API Gutendex
* Armazenar livros (incluindo autor, idioma, número de downloads) no banco de dados
* Listar livros cadastrados
* Listar autores cadastrados
* Consultar autores vivos após um ano específico
* Listar livros por idioma
* Exibir top 10 livros mais baixados
* Mostrar estatísticas gerais do banco (total de livros, autores, downloads, etc.)

## ⚙️ Tecnologias

* Java 21+
* Spring Boot
* Spring Data JPA (Hibernate)
* PostgreSQL
* API pública: Gutendex (JSON)

## 🛠️ Pré-requisitos

* Java 21 (ou superior)
* Maven
* PostgreSQL
* (Opcional) Docker e Docker Compose para rodar o banco

## 🚀 Instalação

1. Clone o repositório

```bash
git clone https://github.com/ZNitr0/challenge-java-literalura-one-g8-main.git
cd challenge-java-literalura-one-g8-main
```

2. Configure o **application.properties** com os dados do PostgreSQL:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
spring.jpa.hibernate.ddl-auto=update
```

3. (Opcional) Inicie o banco usando Docker:

```bash
docker-compose up -d
```

> Exemplos inspirados em projetos como o do Orliluq ([github.com][1], [github.com][2], [github.com][3], [github.com][4]) e luk3mn&#x20;

4. Compile e execute:

```bash
mvn clean install
mvn spring-boot:run
```

## 🧭 Como usar

Ao iniciar, um menu será exibido com opções numeradas:

```
1) Buscar e salvar livro
2) Listar livros cadastrados
3) Listar autores cadastrados
4) Consultar autores vivos após determinado ano
5) Listar livros por idioma
6) Top 10 livros mais baixados
7) Estatísticas do banco
0) Sair
```

Basta digitar o número da opção e seguir as instruções.

## 🎯 Estrutura do projeto

```
src/
 └─ main/java/com/alura/literalura/
     ├─ model/         → entidades (Livro, Autor, etc.)
     ├─ repository/    → interfaces JPA
     ├─ service/       → lógica de negócio
     └─ principal/     → classe com menu e controle de fluxo
src/main/resources/
 └─ application.properties
pom.xml
docker-compose.yml  (opcional)
```

Este layout segue padrões de projetos como os sugeridos por outros participantes da ONE ([github.com][2]).

## 🛡️ Licença

Licenciado sob MIT ou outra licença de sua escolha (caso deseje).

```text
MIT License
```

## 🤝 Contribuição

Contribuições são bem-vindas! Sugestões, correções ou novas funcionalidades são bem-vindas via Issues ou Pull Requests.

## 📞 Contato

Para qualquer dúvida ou feedback:

* LinkedIn: [Levi Do Nascimento](https://www.linkedin.com/in/levi-nascimento-97b599260/)
* GitHub: [@ZNitr0](https://github.com/ZNitr0)


