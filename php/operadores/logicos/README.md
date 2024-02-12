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

[PHP](https://coude-escola.github.io/docs/php/) - [Operadores](https://coude-escola.github.io/docs/php/operadores/)

<!-- referencias -->
## Referências
-  [PHP - OPERADORES LÓGICOS](https://www.php.net/manual/pt_BR/language.operators.logical.php)
<!-- referencias -->

### -> Operadores Lógicos
- !
  ```php
    $comparacao = 8 == '8'; 
    # true
    
    var_dump(!$comparacao);
    # false
  ```
- ||
  ```php
    $comparacao_1 = 8 === '8';
    # false
    $comparacao_2 = 8 < 65;
    # true

    var_dump($comparacao_1 || $comparacao_2);
    # true
  ```
- &&
  ```php
    $comparacao_1 = 8 === '8';
    # false
    $comparacao_2 = 8 < 65;
    # true
    
    var_dump($comparacao_1 && $comparacao_2);
    # false
  ```

<!-- remoção do link inicial -->
  <script>
    onload = ()=>{
      const first_a = document.querySelector('a');
      first_a.style.display = 'none';
    }
  </script>
<!-- remoção do link inicial -->