# Gerenciamento de Funcionários e Setores - Sequelize com SQLite

Este projeto é uma aplicação simples que utiliza o **Sequelize** como ORM (Object Relational Mapper) e **SQLite** como banco de dados. O objetivo é gerenciar informações de **Setores** e **Funcionários**, incluindo suas relações.

---

## 🛠️ Tecnologias Utilizadas

- **Node.js**: Ambiente de execução do JavaScript.
- **Sequelize**: ORM para interação com bancos de dados.
- **SQLite**: Banco de dados leve e simples para aplicações locais.

---

## 📂 Estrutura do Projeto

- **`empresa.sqlite`**: Arquivo do banco de dados SQLite gerado automaticamente.
- **Classes**:
  - **Setor**:
    - Representa os setores da empresa.
    - Campos:
      - `idsetor`: Identificador único do setor.
      - `nome`: Nome do setor.
      - `ramal`: Ramal do setor.
      - `email`: E-mail do setor (opcional).
  - **Funcionario**:
    - Representa os funcionários da empresa.
    - Campos:
      - `matricula`: Identificador único do funcionário.
      - `idsetor`: Relacionamento com o setor (chave estrangeira).
      - `nome`: Nome do funcionário.
      - `nascimento`: Data de nascimento do funcionário (opcional).
      - `telefone`: Telefone do funcionário (opcional).

---

---

## 📊 Funcionalidades

- **Criação do Banco de Dados**:
  - O banco de dados será criado automaticamente no arquivo `empresa.sqlite`.
  - As tabelas `setores` e `funcionarios` serão configuradas de acordo com os modelos definidos.

- **Relacionamento**:
  - Cada funcionário está associado a um setor por meio do campo `idsetor`.

---


