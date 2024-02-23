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

[PHP](/docs/php/) - [Verificadores condicionais](/docs/php/verificadores-condicionais/)

<!-- referencias -->
## Referências
-  [PHP - VERIFICADOR TERNÁRIO](https://www.php.net/manual/pt_BR/control-structures.if.php#Hcom102060)
<!-- referencias -->

## verificador ternário
  ```php
    # o verificador ternário tem um funcionamento similar ao de um conjunto if - else

      # sintaxe
      $retorno = <valor_ou_condicao> ? <retorno_caso_verdadeiro> : <retorno_caso_falso>;

      # ex:

      $situacao = $status_usuario ? 'Ativo' : 'Inativo';
      echo $situacao;

      # ou

      echo $status_usuario ? 'Ativo' : 'Inativo';
  ```

<!-- remoção do link inicial -->
  <script>
    onload = ()=>{
      const first_a = document.querySelector('a');
      first_a.style.display = 'none';
    }
  </script>
<!-- remoção do link inicial -->