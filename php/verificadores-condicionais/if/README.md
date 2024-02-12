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

<!-- referencias -->
## Referências
-  [PHP - IF](https://www.php.net/manual/pt_BR/control-structures.else.php)
-  [PHP - ELSE](https://www.php.net/manual/pt_BR/control-structures.else.php)
<!-- referencias -->

## if
  ```php
      # sintaxe de ação para verdadeiro
      if (<valor_ou_condicao>) {
        # código a ser executado caso o resultado da condição seja verdadeiro
      }

      # ex:

      if($natal){
        echo "Feliz Natal!!!";
      }
  ```

## if / else
  ```php
      # sintaxe de ação para verdadeiro e falso
      if (<valor_ou_condicao>) {
        # código a ser executado caso o resultado da condição seja verdadeiro
      } else {
        # código a ser executado caso o resultado da condição seja falso
      }

      # ex:

      if ($cadastro_realizado) {
        echo "Seu cadastro foi realizado com sucesso!";
      } else {
        echo "Não foi possível realizar o seu cadastro";
      }
  ```

## if / else if
  ```php
      # sintaxe de ação para múltiplas opções de verdadeiros e um falso
      if (<valor_ou_condicao>) {
        # código a ser executado caso o resultado da condição seja verdadeiro
      } else if (<valor_ou_condicao>) {
        # código a ser executado caso o resultado da condição seja verdadeiro
      }

      # ex:

      if ($se_natal) {
        echo "Feliz Natal!";
      
      } else if ($se_pascoa) {
        echo "Feliz Páscoa!";
      
      }
  ```

## if / else if / else
  ```php
      # sintaxe de ação para múltiplas opções de verdadeiros e falso
      if (<valor_ou_condicao>) {
        # código a ser executado caso o resultado da condição seja verdadeiro
      } else if (<valor_ou_condicao>) {
        # código a ser executado caso o resultado da condição seja verdadeiro
      } else {
        # código a ser executado caso o resultado da condição seja falso
      }

      # ex:

      if ($nota_aluno >= 8) {
        echo "Parabéns, você foi aprovado com êxito!";
      
      } else if ($nota_aluno >= 6) {
        echo "Parabéns, você foi aprovado!";
      
      } else {
        echo "Eita! Você não atingiu uma nota de aprovação";
      }
  ```

<!-- remoção do link inicial -->
  <script>
    onload = ()=>{
      const first_a = document.querySelector('a');
      first_a.style.display = 'none';
    }
  </script>
<!-- remoção do link inicial -->