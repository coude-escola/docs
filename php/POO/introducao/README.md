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
    text-decoration: underline;
  }
</style>
# INTRODUÇÃO AO PHP POO
`Classes e Objetos`

Como instânciar e utilizar Classes e Objetos no PHP

[Sumário](/docs/php/)

<!-- referencias -->
## Referências
-  [PHP - POO](https://www.php.net/manual/pt_BR/language.oop5.php)
<!-- referencias -->

## RESUMO
Classes são como moldes / fôrmas, utilizadas para a criação de um Objeto, e o objeto, por sua vez, é a representação

### -> Instância de Uma Classe
A estrutura das Classes compreende basicamente: propriedades e métodos.

```PHP
class MinhaClasse {
  public $propriedade;

  public function verPropriedade(){
    var_dump($propriedade);
  }

  public function setarPropriedade($valor){
    $this->propriedade = $valor
  }
}
```

Observe que no exemplo acima, no método `setarPropriedade`, usamos o termo `$this`. Isso se dá porque não podemos chamar propriedades ou métodos diretamente, sempre que formos chamar precisamos puxar primeiro a classe (ou objeto) onde o valor está contido para depois chamar o valor em si.

Quando estamos no escopo da classe nós a referenciamos como "esta classe", observe: "esta". Por isso o `$this`.

### -> Instância do Objeto
```php
  $meu_objeto = new MinhaClasse();

  $meu_objeto->setarPropriedade("Olá Mundo");
  // a propriedade MinhaClasse::propriedade recebe "Olá Mundo"

  $meu_objeto->verPropriedade();
  // string(9) "Olá Mundo"

  echo $meu_objeto->propriedade;
  // Olá Mundo
```

### -> Herança

Ao criar uma classe que extende outra (`extends`), é herdado, nesta classe filha, todos os valores disponíveis na classe "mãe".

```php
class PrimeiraClasse {
  public $propriedade;

  public function setarPropriedade($valor){
    $this->propriedade = $valor
  }
}

  $primeiro_objeto = new PrimeiraClasse();

  $primeiro_objeto->setarPropriedade("Olá Mundo");
  // a propriedade PrimeiraClasse::propriedade recebe "Olá Mundo"

  echo $primeiro_objeto->propriedade;
  // Olá Mundo

######################################

class SegundaClasse extends PrimeiraClasse{
  // já tenho a $this->propriedade e o $this->setarPropriedade

  public function verPropriedade(){
    var_dump($propriedade);
  }
}

  $segundo_objeto = new SegundaClasse();

  $segundo_objeto->setarPropriedade("Olá Mundo");
  // a propriedade SegundaClasse::propriedade recebe "Olá Mundo"

  $segundo_objeto->verPropriedade();
  // string(9) "Olá Mundo"

  echo $segundo_objeto->propriedade;
  // Olá Mundo
```

### -> Visibilidade

Tanto propriedades quanto métodos de uma classe podem ser `public`, `private` ou `protected`.
- `public`: pode ser acessado por qualquer lugar;
- `private`: só pode ser acessado dentro da classe;
- `protected`: só pode ser acessado dentro da classe e por classes que herdam dela.

```php
class PrimeiraClasse {
  protected $propriedade;

  public function setarPropriedade($valor){
    if(empty($propriedade)){
      $this->propriedade = $valor
    } else {
      return false;
    }
  }
}

  $primeiro_objeto = new PrimeiraClasse();

  $primeiro_objeto->setarPropriedade("Olá Mundo");
  // a propriedade PrimeiraClasse::propriedade recebe "Olá Mundo"

  # echo $primeiro_objeto->propriedade;
  // propriedade não está mais disponível para ser acessada pelo objeto, apenas dentro da classe.

######################################

class SegundaClasse extends PrimeiraClasse{
  // já tenho a $this->propriedade e o $this->setarPropriedade

  private function checaValorPropriedade($novo_valor){
    var_dump($this->propriedade === $novo_valor);

    return !empty($this->propriedade);
  }
  
  public function trocarPropriedade($novo_valor){
    $condicao = $this->checarValorPropriedade($novo_valor);

    if($condicao){
      $this->propriedade = $novo_valor;
    } else {
      return false;
    }
  }
}

  $segundo_objeto = new SegundaClasse();

  $segundo_objeto->setarPropriedade("Olá Mundo"); // método herdado da PrimeiraClasse
  // a propriedade SegundaClasse::propriedade recebe "Olá Mundo"

  $segundo_objeto->trocarPropriedade("Hello World");
  // bool(false)
  // a propriedade SegundaClasse::propriedade recebe "Hello World"

  # echo $primeiro_objeto->propriedade;
  // propriedade não está mais disponível para ser acessada pelo objeto, apenas dentro da classe.
```

<script>
  onload = ()=>{
    const first_a = document.querySelector('a');
    first_a.style.display = 'none';
  }
</script>