# Biblioteca SQLite

Este projeto é um sistema simples de gerenciamento de biblioteca utilizando SQLite. Ele permite o cadastro de autores, livros e registros de empréstimos.

## Funcionalidades

- Cadastro de autores
- Cadastro de livros associados a autores
- Registro de empréstimos de livros

## Estrutura do Banco de Dados

O banco de dados é composto por três tabelas:

- **Autores**
  - AutorID (chave primária)
  - Nome
  - Nacionalidade

- **Livros**
  - LivroID (chave primária)
  - Titulo
  - AutorID (chave estrangeira referenciando Autores)
  - AnoPublicacao
  - Genero

- **Emprestimos**
  - EmprestimoID (chave primária)
  - LivroID (chave estrangeira referenciando Livros)
  - DataEmprestimo
  - DataDevolucao
  - NomeUsuario

## Como Usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/biblioteca-sqlite.git
   cd biblioteca-sqlite
