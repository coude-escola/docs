<!-- coloração da página -->
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
<!-- coloração da página -->

[Sumário](/docs/sql/) > [DDL](/docs/sql/ddl/) > Banco de Dados

<!-- referencias -->
## Referências
- [Link documentação externa](https://###.com)
- [Link documentação externa](https://###.com)
- [Link documentação externa](https://###.com)
- [Link documentação externa](https://###.com)
<!-- referencias -->

### CRIA O BANCO 
```SQL
create database `cadastro`; 
```

### CRIA O BANCO SE NÃO EXISTIR OUTRO COM MESMO NOME 
```SQL
create database if not exists `cadastro`;
```

### EXCLUI DO BANCO SE EXISTIR
```SQL
drop database `cadastro`;
-- ou
drop database if exists `cadastro`; -- garante a exclusão do banco apenas caso ele exista
```


#### Exercícios:
1. Crie um banco de dados chamado EntretenimentoDB. Em seguida, exclua esse banco de dados.

2. Crie um banco de dados chamado BibliotecaDB. Verifique a criação listando todos os bancos de dados. Depois, exclua o banco de dados.

3. Crie um banco de dados chamado EscolaDB e um banco de dados chamado HospitalDB. Liste todos os bancos de dados e exclua o HospitalDB.

<!-- remoção do link inicial -->
  <script>
    onload = ()=>{
      const first_a = document.querySelector('a');
      first_a.style.display = 'none';
    }
  </script>
<!-- remoção do link inicial -->