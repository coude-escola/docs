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
-  [PHP - SWITCH](https://www.php.net/manual/pt_BR/control-structures.switch.php)
<!-- referencias -->

## switch
  ```php
      # o switch se assemelha a um conjunto if - else if - else

      # sintaxe
      switch(<valor_a_ser_comparado>){
        case <primeira_opcao>:
          # código corresponden
          break;
        case <segunda_opcao>:
          # código corresponden
          break;
        default:
          # código corresponden caso nenhuma opção seja atendida
          break;
      }

      # ex:
      
      switch($tipo_conta){
        case 'ouro':
          echo "Você é um usuário OURO";
          break;
        case 'prata':
          echo "Olha só! Sua conta é PRATA";
          break;
        case 'bronze':
          echo "Que massa! Sua conta é do tipo Bronze";
          break;
        default:
          echo "Não foi possível identificar o tipo da sua conta. Por gentileza contate o suporte.";
          break;
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