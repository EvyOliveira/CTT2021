# Lista de Exercícios V

> À partir do dia 25 de fevereiro com foco em funções síncronas, de calculadora simples, desafio do número perfeito e números primos.

```js

// Criar uma function que recebe dois números [n1, n2] por parâmetro e retorna a soma dos dois números e atribuir esta função para uma variável constante chamada somar.

// Função síncrona
const soma = function DoisNumeros (n1, n2) {
    return n1 + n2
}

// Arrow function
const soma = (n1, n2) => n1 + n2

console.log(soma(1,1))

// Criar uma function que recebe dois números [n1, n2] por parâmetro e retorna a subtração dos dois números e atribuir esta função para uma variável constante chamada subtrair.

// Função síncrona
const subtracao = function DoisNumeros (n1, n2) {
    return n1 - n2
}

// Arrow function
const sobtração = (n1, n2) => n1 - n2

console.log(subtracao(1,1))

// Criar uma function que recebe dois números [n1, n2] por parâmetro e retorna a subtração dos dois números e atribuir esta função para uma variável constante chamada subtrair.

// Função síncrona
const divisao = function DoisNumeros (n1, n2) {
    return n1 / n2
}

// Arrow function
const divisao = (n1, n2) => n1 / n2

console.log(divisao(1,1))

// Criar uma function que recebe dois números [base, expoente] por parâmetro e retorna o valor da base elevada ao expoente e atribuir esta função para uma variável constante chamada calcularPotencia.

// Função síncrona
const potencia = function DoisNumeros (base, expoente) {
    return base ** expoente
}

// Arrow function
const calcularPotencia = (base, expoente) => {
	const resultado = base ** expoente
return resultado
}

console.log(calcularPotencia(3,3))

// Criar uma function que recebe um número [n por parâmetro e calcula a porcentagem deste número e atribuir esta função para uma variável constante chamada calcularPorcentagem. Exemplo: 10% == 0.1.

// Função síncrona
const porcentagem = function DoisNumeros (n) {
    return n = n/100
return console.log(n + '%')
}

const calcularPorcentagem = 
	function(n) {
	return n/100;
}

console.log(calcularPorcentagem(10))

// Desafio Número Perfeito: Um número é dito perfeito quando ele é igual a soma de seus fatores. Por exemplo: 6 = 1 + 2 + 3, ou seja, podemos dividir 6 por 1, 6 por 2 e 6 por 3. Sendo assim 6 é um número perfeito. 

// Subitem 1: Implemente uma função que recebe um número [n] por parâmetro e identifica se n é um número perfeito. P.S.: Atribuir esta função para uma variável constante chamada ehNumeroPerfeito.

// Subitem 2: Se o número for perfeito, imprimir a mensagem ‘O número n é um número perfeito’ onde na mensagem ‘n’ deve ser substituído pelo número que chegou pelo parâmetro n; Dica: Pesquisar sobre Template String em JS para imprimir a mensagem.

// Subitem 3: Se o número NÃO for perfeito, imprimir a mensagem ‘O número n NÃO é um número perfeito’ onde na mensagem ‘n’ deve ser substituído pelo número que chegou pelo parâmetro n; Dica: Pesquisar sobre Template String em JS para imprimir a mensagem.

// Subitem 4: Implementar as validações utilizando apenas if (sem else, sem else-if, sem switch).

const ehNumeroPerfeito = (n) => {
  let soma = 0;

  for(let index = 1; index < n; index++) {
    if ((n % index) === 0) {
      soma += index;
    }
  }

  if (soma === n) {
    console.log(`O número ${n} é um número perfeito`)
  }

  if (soma !== n) {
    console.log(`O número ${n} NÃO é um número perfeito`)
  }

}

// Desafio Números Primos: Um número é considerado primo quando ele é divisível apenas por 1 e por ele mesmo.

// Subitem 1: Implemente uma função que recebe um número [n] por parâmetro e identifica se n é um número primo. P.S.: Atribuir esta função para uma variável constante chamada ehPrimo.

// Subitem 2: Se o número for perfeito, imprimir a mensagem ‘O número n é um número perfeito’ onde na mensagem ‘n’ deve ser substituído pelo número que chegou pelo parâmetro n. Dica: Pesquisar sobre Template String em JS para imprimir a mensagem.

// Subitem 3: Se o número NÃO for perfeito, imprimir a mensagem ‘O número n NÃO é um número perfeito’ onde na mensagem ‘n’ deve ser substituído pelo número que chegou pelo parâmetro n. Dica: Pesquisar sobre Template String em JS para imprimir a mensagem.
?

```