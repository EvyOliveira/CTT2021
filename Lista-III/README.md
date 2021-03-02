# Lista de Exercícios III

> À partir do dia 23 de fevereiro. Aula de introdução ao JavaScript com foco em tipos de variáveis.  

```js

// Item 1: Criar uma variável de escopo global ou função e que pode ter seu valor alterado.
var teste = 1
console.log(teste)

var teste = 2
console.log(teste)
// 1
// 2
// undefined

// Item 2: Criar uma variável de escopo de bloco ou função e que NÃO pode ter seu valor alterado.

// Subitem 1 do Item 2: Tentar alterar o valor dessa variável e ver o que acontece.
const teste = 1
console.log(teste)

const teste = 2
console.log(teste)
// 1
// undefined
// Uncaught SyntaxError: Identifier 'teste' has already been declared
  // at <anonymous>:1:1

// Item 3: Criar uma variável de escopo de bloco ou função e que pode ter seu valor alterado.
let teste = 1
console.log(teste)

let teste = 2
console.log(teste)
// 1
// 2
// undefined

// Item 4: Criar uma variável de escopo de bloco ou função e que NÃO pode ter seu valor alterado, inicializando a mesma com o valor = 10.

// Subitem 1 do Item 4: Tenta alterar esse valor para 5.
const valor = 10
console.log(valor)
// 10

valor = 5
console.log(valor)
// Uncaught TypeError: Assignment to constant variable.
  // at <anonymous>:1:7

// Item 5: Criar uma variável de escopo global ou função e que pode ter seu valor alterado, inicializando a mesma com o valor = 10.

// Subitem 1 do Item 5: Tentar alterar esse valor para string ⇒ 'teste'.
let valor = 10
console.log(valor)
// 10

valor = 'teste'
console.log(valor)
// 'teste'

// Item 6: Criar uma variável de escopo global ou função e que pode ter seu valor alterado. Inicializando a mesma com o valor undefined. 

// Subitem 1 do Item 6: Tentar alterar esse valor para null.
var val = undefined
console.log(val)
// undefined
// undefined

var val = null
console.log(val)
// null
// undefined

// Item 7: Criar uma variável de escopo de bloco ou função e que NÃO pode ter seu valor alterado, com o nome de objetoTeste, inicializando a mesma com o valor ⇒ {}. 

// Subitem 1 do Item 7: Tentar alterar esse valor para null.
const objetoTeste = {}
console.log(objetoTeste)
// {}

const objetoTeste = null
console.log(objetoTeste)
// null
// undefined

// Subitem 2: Tentar incluir uma propriedade neste objeto da seguinte forma: objetoTeste.a = 10.
objetoTeste.a = 10;
// 10
console.log(objetoTeste)
// {a: 10}

// Subitem 3: Tentar alterar o valor da propriedade a para = 5.
objetoTeste.a = 5;
console.log(objetoTeste)
// {a: 5}
// undefined

// Subitem 4: Tentar incluir uma propriedade nome neste objeto, inicializando com o valor 'teste'.
objetoTeste.nome = 'teste';
console.log(objetoTeste)
// {a: 5, nome: "teste"}
// undefined

```
