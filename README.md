# 📜 Criação de Funções em JavaScript

## 📌Sobre
- As funções são fundamentais dentro das linguagens de programação e o JavaScript não está fora disso. Uma função é um conjunto de instruções determinadas pelo programador e essas funções só serão executadas apenas quando forem chamadas e são utilizadas para evitar a repetição de códigos.

# 📝 Declaração de Função
- Para declarar uma função é preciso escrever a palavra-chave ***function*** e em seguida o nome dessa função, entre parenteses, um ou mais paramentos separados por vírgulas e ao final a colocação de chaves ***{ }***, é dentro delas que iremos colocar nossas instruções.
  
```JavaScript
function soma(numero){
  return numero + numero;
};
console.log(soma(2));
```
### Vantagens:
- Uma das principais vantagens de declarar funções é deixar o escopo do seu código mais limpo e evitando repetição de códigos, deixando o ambiente poluído.
### Desvantagens:
- E uma das desvantagens é a sobrecarga da memória, que pode consumir memória, especialmente se forem chamadas muitas vezes.

# 🔄 Expressão de Função
- Também é possível criar funções através de expressões de função, onde a função (pode ser anônima ou nomeada) é atribuída a uma variável.
  
```JavaScript
let soma = function (numero){
  return numero + numero;
};
let recebeSoma = soma;
```

### Vantagens:
- A expressão de função oferece algumas vantagens como evitar poluição do escopo global, facilitando a reutilização de códigos e tornando o código mais limpo e organizado.

### Desvantagens:
- Porém, também apresenta certas desvantagens, sendo mais difícil de depurar, problemas com autorreferência entre outros.

# ➡️ Arrow Functions

- As Arrows function no JavaScript são uma forma mais resumível escrever certas funções. Uma das principais mudanças dentro das Arrows Function é que não é necessário utilizar a palavra-chave ***function***. Porém, definimos as variáveis como constantes e usamos a função como seu valor. Além disso, dentro das Arrows Function iremos utilizar o sinal ***=>(seta)*** para definir a instrução da função e o valor que ela irá retornar.

```JavaScript
const subtracaoVersao2 = (a, b) => a - b;

const somar2Versao2 = a => a + 2;
```

### Vantagens:
- Ele tem uma sintaxe concisa, tem um retorno implícito e permite um código mais limpo e legível.

### Desvantagens:
- Não possuem *This* ou *arguments*, dificuldade de depuração e não são adequadas para métodos.
