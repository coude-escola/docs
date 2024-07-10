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

[Sumário](/docs/sql/) > [DDL](/docs/sql/ddl/) > Criação de Tabelas

<!-- referencias -->
## Referências
- [Link documentação externa](https://###.com)
- [Link documentação externa](https://###.com)
- [Link documentação externa](https://###.com)
- [Link documentação externa](https://###.com)
<!-- referencias -->

### INFORMA O BANCO QUE SERÁ UTILIZADO (NECESSÁRIO APENAS NO INÍCIO DA MANIPULAÇÃO)
```SQL
use seu_banco;
-- ou 
create table seu_banco.sua_tabela(
  -- coluna1 tipo1,
  -- coluna2 tipo2
);
```

### CRIAÇÃO DE TABELA SIMPLES
```SQL
create table pessoa (
  nome varchar(30),          -- STRING (texto) DE TAMANHO VARIÁVEL
  idade int,                 -- VALOR NUMÉRICOS INTEIRO 
  sexo char(1),              -- STRING (texto) DE TAMANHO FIXO
  peso float,                -- VALOR NUMÉRICO FRACIONADO
  estatura float,            -- VALOR NUMÉRICO FRACIONADO
  nacionalidade varchar(30)  -- STRING (texto) DE TAMANHO VARIÁVEL
);
```

### APRESENTA A ESTRUTURA DA TABELA
```SQL
  describe pessoa;
```

1. No banco de dados EntretenimentoDB, crie uma tabela chamada Filmes com as colunas ID (inteiro, chave primária), Nome (varchar), e Genero (varchar).

2. No banco de dados BibliotecaDB, crie uma tabela chamada Livros com as colunas ISBN (varchar, chave primária), Titulo (varchar), e Autor (varchar).

3. No banco de dados EscolaDB, crie uma tabela chamada Alunos com as colunas AlunoID (inteiro, chave primária), Nome (varchar), Sobrenome (varchar), e DataMatricula (data).


<!-- remoção do link inicial -->
  <script>
    onload = ()=>{
      const first_a = document.querySelector('a');
      first_a.style.display = 'none';
    }
  </script>
<!-- remoção do link inicial -->