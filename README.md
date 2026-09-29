# JDBC DAO Pattern

Aplicação Java desenvolvida para praticar acesso a banco de dados utilizando JDBC e o padrão DAO (Data Access Object), com persistência de dados em MySQL.

O projeto foi desenvolvido com foco na compreensão do acesso direto ao banco de dados em Java, separação de responsabilidades e implementação de uma camada de acesso a dados.

## 🚀 Tecnologias

- Java
- JDBC
- MySQL

## 📚 Conceitos praticados

- Conexão com banco de dados utilizando JDBC
- Padrão DAO (Data Access Object)
- Separação de responsabilidades
- Acesso e persistência de dados
- Operações com banco de dados
- Tratamento de exceções relacionadas ao banco
- Organização da camada de acesso a dados
- Implementação de interfaces e classes DAO
- Factory Pattern para criação de objetos DAO

## 🏗️ Estrutura do projeto

O projeto utiliza uma organização baseada no padrão DAO, separando as entidades da camada responsável pelo acesso aos dados:

- **Application** — classes responsáveis pela execução e testes da aplicação
- **DB** — gerenciamento da conexão com o banco de dados e tratamento de exceções
- **Entities** — representação dos objetos do domínio
- **DAO** — interfaces responsáveis pelas operações de acesso aos dados
- **DAO/Impl** — implementações concretas dos DAOs
- **DaoFactory** — responsável pela criação das implementações dos DAOs

## 🗂️ Entidades

O projeto possui as seguintes entidades:

- **Department**
- **Seller**

## 🗄️ Banco de dados

O projeto utiliza **MySQL** para persistência dos dados.

Configuração utilizada:

- Banco de dados: `coursejdbc`
- Host: `localhost`
- Porta: `3306`
- Acesso ao banco: JDBC

As credenciais do banco são configuradas localmente através do arquivo:

```text
db.properties
```

Por motivos de segurança, esse arquivo não é versionado no repositório.

Utilize o arquivo `db.properties.example` como referência para configurar o acesso ao banco:

```properties
user=SEU_USUARIO
password=SUA_SENHA
dburl=jdbc:mysql://localhost:3306/coursejdbc
useSSL=false
```

## ⚙️ Como executar

### Pré-requisitos

- Java
- MySQL
- Eclipse ou outra IDE compatível com projetos Java

### 1. Clone o repositório

```bash
git clone https://github.com/guisbezerra/jdbc-dao-pattern.git
```

### 2. Configure o banco de dados

Crie o banco de dados `coursejdbc` no MySQL.

Depois, crie o arquivo `db.properties` na raiz do projeto com suas credenciais:

```properties
user=SEU_USUARIO
password=SUA_SENHA
dburl=jdbc:mysql://localhost:3306/coursejdbc
useSSL=false
```

### 3. Execute a aplicação

Abra o projeto em sua IDE Java e execute uma das classes disponíveis no pacote `application`.

## 🎯 Objetivo

Projeto desenvolvido para consolidar conhecimentos em Java e JDBC, explorando o padrão DAO, acesso direto ao banco de dados, separação de responsabilidades e organização de uma aplicação Java com persistência em MySQL.
