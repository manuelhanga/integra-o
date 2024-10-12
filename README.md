# Biblioteca SQLite

Este projeto é um sistema simples de gerenciamento de uma biblioteca utilizando um banco de dados SQLite. Ele permite a inserção e consulta de autores, livros e empréstimos.

## Estrutura do Banco de Dados

O banco de dados contém três tabelas:

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

1. Certifique-se de ter o Python e o SQLite instalados em sua máquina.
2. Clone este repositório:
   ```bash
   git clone <URL do repositório>
