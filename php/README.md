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
# INTRODUÇÃO AO PHP
`VALORES, VARIÁVEIS E CONSTANTES`

Conhecendo tipos de valores, instância de variáveis e constantes e operadores no PHP.

<!-- referencias -->
## Referências
-  [PHP - TIPOS DOS VALORES](https://www.php.net/manual/pt_BR/language.types.intro.php)
-  [PHP - DEFINIÇÃO DE VARIÁVEIS](https://www.php.net/manual/pt_BR/language.variables.basics.php)
-  [PHP - DEFINIÇÃO DE CONSTANTES](https://www.php.net/manual/pt_BR/language.constants.syntax.php)
-  [PHP - ACRÉCIMO E DECRÉCIMO](https://www.php.net/manual/pt_BR/language.operators.increment.php)
-  [PHP - OPERADORES DE ATRIBUIÇÃO](https://www.php.net/manual/pt_BR/language.operators.assignment.php)
<!-- referencias -->

## RESUMO

Vocês verão que existem alguns valores que não foram exibidos aqui. Isso ocorre por dois motivos:
 1) Preferenciamos o que é mais usual;
 2) Preferenciamos o que mais se assemelha a outras linguagens. 

### -> Tipos de Valores
- Null . . . . . . `Vazio`
- Boll . . . . . . `Verdadeiro ou Falso`
- Number . . `Numérico`
- String . . . .  `Textos`
- Array . . . . .`Coleção / Matriz`
- Object . . . .`Objeto`

### -> Instância de Variáveis
```php
  # $nome_da_variavel = <valor>;
    $null = null;
    $boll = true;
    $number_int = 5;
    $number_float = 6.75;
    $string = 'valor';
    $array = ['valor_1', 'valor_2', 'valor_3', 'valor_4'];
```

### -> Instância de Constantes
```php
  # define('<nome_da_constante>', <valor_da_constante>);
  
  define('DB_HOST', 'localhost');
  define('DB_USER', 'root');
  define('DB_PASS', '');
  define('DB_NAME', 'mydb');
```

<script>
  onload = ()=>{
    const first_a = document.querySelector('a');
    first_a.style.display = 'none';
  }
</script>