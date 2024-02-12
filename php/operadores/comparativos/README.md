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
-  [PHP - OPERADORES DE COMPARAÇÃO](https://www.php.net/manual/pt_BR/language.operators.comparison.php)
<!-- referencias -->

### -> Operadores Comparativos
- Igual:
  ```php
  var_dump(8 == '8');
  # true
  ```
- Diferente:
  ```php
  var_dump(8 != 8);
  # false
  ```
- Idêntico:
  ```php
  var_dump(0 === false);
  # false
  ```
- Não identico:
  ```php
  var_dump(0 !== false);
  # true
  ```
- Menor que:
  ```php
  var_dump(6 < 8);
  # true
  ```
- Menor ou igual a:
  ```php
  var_dump(8 <= 8);
  # true
  ```
- Maior que:
  ```php
  var_dump(8 > 8);
  # false
  ```
- Maior ou igual a:
  ```php
  var_dump(9 >= 8);
  # true
  ```

<!-- remoção do link inicial -->
  <script>
    onload = ()=>{
      const first_a = document.querySelector('a');
      first_a.style.display = 'none';
    }
  </script>
<!-- remoção do link inicial -->