# 📜 Criação de Funções em JavaScript

## 📌Sobre
- As funções são fundamentais dentro das linguagens de programação e o JavaScript não está fora disso. Uma função é um conjunto de instruções determinadas pelo programador e essas funções só serão executadas apenas quando forem chamadas e são utilizadas para evitar a repetição de códigos.

# 📝 Declaration Function
⮞ Para declarar uma função é preciso escrever a palavra-chave ***function*** e em seguida o nome dessa função, entre parenteses, um ou mais paramentos separados por vírgulas e ao final a colocação de chaves ***{ }***, é dentro delas que iremos colocar nossas instruções.
  
```JavaScript
function soma(numero){
  return numero + numero;
};
console.log(soma(2));
```
```JavaScript
function media(numero1, numero2, numero3) {
  return (numero1 + numero2 + numero3) / 3;
};
console.log(media(5, 8, 9));
```
```JavaScript
function impar_Par(numero){
  return numero % 2 == 0;
};
console.log(2);
console.log(3);
```
### Vantagens:
- Uma das principais vantagens de declarar funções é deixar o escopo do seu código mais limpo e evitando repetição de códigos, deixando o ambiente poluído.
### Desvantagens:
- E uma das desvantagens é a sobrecarga da memória, que pode consumir memória, especialmente se forem chamadas muitas vezes.

# 🔄 Expression Function
⮞ Também é possível criar funções através de expressões de função, onde a função (pode ser anônima ou nomeada) é atribuída a uma variável.
  
```JavaScript
let soma = function (numero) {
  return numero + numero;
};

let recebeSoma = soma;

console.log(soma(5));        // 10
console.log(recebeSoma(8));  // 16
```
```JavaScript
let media = function(numero1, numero2, numero3) {
  return (numero1 + numero2 + numero3) / 3;
};

let recebaMedia = media(5, 8, 9);
console.log(recebaMedia); // Saída: 7.33
```
```JavaScript
let impar_Par = function(numero) {
  return numero % 2 == 0;
};

let resultadoImpar_Par1 = impar_Par(2); // true
let resultadoImpar_Par2 = impar_Par(3); // false

console.log(resultadoImpar_Par1); // true
console.log(resultadoImpar_Par2); // false
```

### Vantagens:
- A expressão de função oferece algumas vantagens como evitar poluição do escopo global, facilitando a reutilização de códigos e tornando o código mais limpo e organizado.

### Desvantagens:
- Porém, também apresenta certas desvantagens, sendo mais difícil de depurar, problemas com autorreferência entre outros.

# ➡️ Arrow Functions

⮞ As Arrows function no JavaScript são uma forma mais resumível escrever certas funções. Uma das principais mudanças dentro das Arrows Function é que não é necessário utilizar a palavra-chave ***function***. Porém, definimos as variáveis como constantes e usamos a função como seu valor. Além disso, dentro das Arrows Function iremos utilizar o sinal ***=>(seta)*** para definir a instrução da função e o valor que ela irá retornar.

```JavaScript
const subtracaoVersao2 = (a, b) => a - b;
const somar2Versao2 = a => a + 2;

console.log(subtracaoVersao2(10, 4)); // 6
console.log(somar2Versao2(5));        // 7
```
```JavaScript
const media = (numero1, numero2, numero3) => (numero1 + numero2 + numero3) / 3;

console.log(media(5, 8, 9)); // Saída: 7.333...
```
```JavaScript
let impar_Par = (numero) => numero % 2 == 0;
console.log(impar_Par(2)); //true
console.log(impar_Par(3)); //false
```
### Vantagens:
- Ele tem uma sintaxe concisa, tem um retorno implícito e permite um código mais limpo e legível.

### Desvantagens:
- Não possuem *This* ou *arguments*, dificuldade de depuração e não são adequadas para métodos.
