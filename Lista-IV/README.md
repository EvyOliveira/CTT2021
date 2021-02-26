# Lista de Exercícios IV

> À partir do dia 24 de fevereiro com foco em funções síncronas. 

```js

// Criar uma function que imprima a string 'Hello Word!'.
function imprimaMensagem () {
	console.log('Hello World')
}
imprimaMensagem()

// Criar uma function que receba um parâmetro [nome] e imprima a string 'Hello' + o valor do parâmetro. 
var nome = 'Evelyn';

function mensagem (nome) {
	console.log('Hello ' + this.nome)
}
mensagem()

// Item: Criar uma function que receba dois números por parâmetro [n1, n2], retornar a soma dos dois números e imprimir o valor retornado da função. Atribuir esta função para uma variável.
?

// Subitem 1: Se os dois valores forem do tipo Number, executar a subtração dos valores, retornar o resultado da subtração e imprimir o valor retornado da função.
?

// Subitem 2: Se algum dos dois parâmetros for DIFERENTE do tipo Number, então retornar null e imprimir o valor retornado da função.
?

// Item: Criar uma function chamada funcaoRecursiva que recebe um número n por parâmetro e executa a seguinte lógica:

// Subitem 1: Se n <= 0, então retorna uma string 'Fim da execução'.
?

// Subitem 2: Se n> 0, então devemos imprimir o valor de n e chamar novamente a função funcaoRecursiva passando por parâmetro [n - 1].
?

// Item: Criar uma function chamada fizzBuzzRecursivo que recebe um número n por parâmetro e executa a seguinte lógica:

// Subitem 1: Se n <= 0, então retorna uma string 'Fim da execução'.
?

// Subitem 2: Se n for multíplo de 3, então imprimir a string 'Fizz' e chamar novamente a função fizzBuzzRecursivo passando por parâmetro [n - 1].
?

// Subitem 3: Se n for multíplo de 5, então imprimir a string 'Buzz' e chamar novamente a função fizzBuzzRecursivo passando por parâmetro [n - 1].
?

// Subitem 4: Se n for multíplo de 3 e multiplo de 5, então imprimir a string 'FizzBuzz' e chamar novamente a função fizzBuzzRecursivo passando por parâmetro [n - 1].
?

// Subitem 5: Se não for múltiplo de 3 e não for múltiplo de 5, então imprimir o valor de n e chamar novamente a função fizzBuzzRecursivo passando por parâmetro [n - 1].
?

```