<style>
  body{
    background-color: #373737;
    color: #c5c5c5;
  }
  code{
    color: #507d9f;
  }
</style>
# INTRODUÇÃO AO PHP

Conhecendo tipos de valores, instância de variáveis e constantes e operadores no PHP.


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

### -> Operadores Aritiméticos
  - Adição
    ```php
      echo 8 + 8;
      # 16
    ```
  - Subtração
    ```php
      echo 7 - 5;
      # 2
    ```
  - Multiplicação
    ```php
      echo 3 * 25;
      # 75
    ```
  - Divisão
    ```php
      echo 144 / 12;
      # 12
    ```
  - Resto da Divisão
    ```php
      echo 345678 % 2;
      # 0
    ```
  - Potências
    ```php
      echo 3 ** 2;
      # 9
    ```

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

### -> Verificadores Condicionais
  - if / else if / else
```php
    # sintaxe de ação para verdadeiro
    if (<valor_ou_condicao>) {
      # código a ser executado caso o resultado da condição seja verdadeiro
    }

    # ex:

    if($natal){
      echo "Feliz Natal!!!";
    }

    #=====================================#

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

    #=====================================#

    # sintaxe de ação para múltiplas opções de verdadeiros e um falso
    if (<valor_ou_condicao>) {
      # código a ser executado caso o resultado da condição seja verdadeiro
    } else if (<valor_ou_condicao>) {
      # código a ser executado caso o resultado da condição seja verdadeiro
    }

    #=====================================#

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

### -> Verificador Ternário
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
  - switch
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
<script>
  onload = ()=>{
    const first_a = document.querySelector('a');
    first_a.style.display = 'none';
  }
</script>
