<style>
  body{
    background-color: #373737;
    color: #c5c5c5;
  }
  code{
    color: #507d9f;
  }
  a{
    color: #eee;
    text-decoration:underline;
  }
</style>
# INTRODUÇÃO AO SQL
`O QUE É, PARA QUE SERVE`

Conhecendo as características fundamentais do SQL.

[Sumário](/docs/sql/)

<!-- referencias -->
## Referências
-  [LINK](#)
-  [LINK](#)
-  [LINK](#)
-  [LINK](#)
<!-- referencias -->

## RESUMO

SQL (Structured Query Language) é uma linguagem de programação padronizada usada para gerenciar e manipular bancos de dados relacionais. Ela permite que os usuários executem várias operações em dados armazenados em bancos de dados, como inserir, consultar, atualizar e excluir registros.

Nesse material veremos 3 dos 5 usos gerais do SQL: DDL, DML, DQL.

### -> [DDL (Data Definition Language)](/docs/sql/ddl/)
Define a estrutura do banco de dados, incluindo a criação, alteração e exclusão de tabelas e outros objetos de banco de dados.

**Exemplos de comandos:**
- *CREATE*: Cria uma nova tabela ou outro objeto no banco de dados.
- *ALTER*: Altera a estrutura de uma tabela existente.
- *DROP*: Remove uma tabela ou outro objeto do banco de dados.
- *TRUNCATE*: Remove todos os registros de uma tabela, mas mantém a estrutura da tabela.

### -> [DML (Data Manipulation Language)](/docs/sql/dml/)
Manipula os dados dentro das tabelas, permitindo a inserção, atualização, exclusão e recuperação de dados.

**Exemplos de comandos:**
- *INSERT*: Insere novos registros em uma tabela.
- *UPDATE*: Atualiza registros existentes em uma tabela.
- *DELETE*: Exclui registros de uma tabela.

### -> [DQL (Data Query  Language)](/docs/sql/dql/)
Realiza consultas para recuperar dados armazenados no banco de dados.

**Exemplos de comandos:**
- *SELECT*: Recupera dados de uma ou mais tabelas. Este é o comando principal usado para consultar dados em um banco de dados.


<script>
  onload = ()=>{
    const first_a = document.querySelector('a');
    first_a.style.display = 'none';
  }
</script>