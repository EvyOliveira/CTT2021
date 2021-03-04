# Lista de Exercícios VII

> À partir do dia 27 de fevereiro. Exercícios sobre promises, async/await, objetos, arrays bem como suas principais operações.

#### Exercício de funções assíncronas com Promise

```js

// Item 1: Criar uma contante com o nome [idade] e inicializar com o valor 14.

// Subitem 1: Criar uma promise que recebe por parâmetro uma function, que recebe dois parâmetro [resolve, reject]. Dentro dessa function que recebe resolve, reject, implementar uma lógica para saber se a idade é maior ou menor que 18.

// Item 1 do subitem 1: Se idade > 18, então invocar a função resolve passando a mensagem ['Pessoa maior de idade'] por parâmetro.

// Item 2 do subitem 1: Se não, invocar a função reject passando a mensagem ['Pessoa MENOR de idade'] por parâmetro.

// Item 2: Após implementar esta promise, executar a mesma e imprimir a mensagem retornada, seja de sucesso ou de erro.
const idade = 14

const promise = new Promise (function (resolve, reject) {
	if (idade > 18) {
// Não precisa necessaramente, passar o resolve com o return. É só um caminho.
		return resolve('Pessoa maior de idade.')
	}
	reject('Pessoa MENOR de idade.');
	return;
})

promise
	.then((resultado) => console.log('Sucesso: ', resultado))
	.catch((resultado) => console.log('Erro: ', resultado))

```

#### Exercício de funções assíncronas com Async/await

```js

// Item 3: Criar uma função async que recebe por parâmetro um número n e executar uma lógica para saber se a n é maior ou menor que 18.

// Subitem 1 do item 3: Se n > 18, então retornar a mensagem ['Pessoa maior de idade'] por parâmetro.

// Subitem 2 do item 3: Se n < 18, retornar a mensagem ['Pessoa MENOR de idade'] por parâmetro.

// Subitem 3: Após implementar essa function, invocar a mesma e imprimir a mensagem retornada.
(async () => {
async function verificaIdade(n) {
	if (n > 18) {
		return 'Pessoa maior de idade.'
	}
	return 'Pessoa MENOR de idade.';
	}

const resultado = await verificaIdade(17)
console.log(resultado)
})()

```

#### Exercício de objetos

```js

// Item 4: Criar um objeto pessoa.

// Subitem 1: Adicionar a propriedade nome com valor 'juca' utilizando a notação de ponto.

// Subitem 2: Adicionar a propriedade idade com valor 21 utilizando a notação de ponto.

// Subitem 3: Adicionar a propriedade ehMaiorDeIdade com valor function utilizando a notação de ponto. A function ehMaiorDeIdade deve ser a lógica:

// Subitem 1 do item 4: Se this.idade ≥ 18, então return true.

// Subitem 1 do item 4: Se não, return false.

// Subitem 4: Após criar o objeto, chamar a function ehMaiorDeIdade e imprimir o resultado.
const pesssoa = {}

pessoa.nome = 'juca'
pessoa.idade = 21
pessoa.ehMaiorDeIdade = function () {
	if (this.idade >= 18) return true;
	return false
}

console.log(pessoa)

console.log(pessoa.EhMaiorDeIdade())

pessoa.idade = 10

console.log(pessoa)

console.log(pessoa.EhMaiorDeIdade())

// Item 5: Criar um novo objeto pessoa nomeando como pessoa2.

// Subitem 1: Adicionar a propriedade nome com valor 'joão' utilizando a notação de colchete.

// Subitem 2: Adicionar a propriedade idade com valor 12 utilizando a notação de colchete.

// Subitem 3: Adicionar a propriedade dizOla com valor function utilizando a notação de colchete. 

// Item 1 do subitem 3: OBS: A function deve ser escrita utilizando notação de arrow function.

// Item 2 do subitem 3: OBS: A function deve receber um objeto pessoa por parâmetro.

// Item 3 do subitem 3: Ao invocar a função dizOla, deve retornar a mensagem: Ola [nome da pessoa], meu nome é João.

// Subitem 4: Após criar o objeto, chamar a function dizOla (utilizando a notação de colchete) e imprimir o resultado.
const pesssoa = {}
const pessoa2 = {};

pessoa.nome = 'juca';
pessoa.idade = 21;
pessoa.ehMaiorDeIdade = function () {
	if (this.idade >= 18) return true;
	return false;
}

console.log(pessoa)

//console.log(pessoa.EhMaiorDeIdade())

//pessoa.idade = 10

//console.log(pessoa)

//console.log(pessoa.EhMaiorDeIdade())

pessoa2['nome'] = 'joão';
pessoa2['idade'] = 21;
pessoa2['dizOla'] = (pessoaCustom) => `Olá ${pessoaCustom.nome}, meu nome é joão. Você é maior de idade: ${pessoaCustom.ehMaiorDeIdade()}`;

console.log(pessoa2) 

console.log(pessoa2['dizOlá'](pessoa))

pessoa.nome = 'Leo'
//pessoa.idade = 8

console.log(pessoa) 

console.log(pessoa2['dizOlá'](pessoa))

```

#### Exercício de Arrays - for e for of

```js

// Item 6: Criar um array com 10 números e percorrer o array utilizando for, imprimir todos os números do array dentro do for. 
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

for (let i = 0; i < array.length; i++) {
	console.log(array[i])
}

// Item 7: Criar um array com 10 números e percorrer o array utilizando for, imprimir a todos os números do array multiplicado por 2. Exemplo: n * 2 (n representa cada número do array) dentro do for.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

for (let i = 0; i < array.lenght; i++) {
	console.log(array[i] * 2)
}

// Item 8: Criar um array com 10 números e percorrer o array utilizando o for. Transformar todos os itens do array em string e imprimir todos os números do array dentro do for.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

for (let i = 0; i < array.lenght; i++) {
	const string = `${array[i]}`
	console.log(string)
}

// Item 9: Criar um array com 10 números e percorrer o array utilizando for. Somar todo os números e ao final da execução do for, imprimir o resultado da soma.
?

// Item 10: Criar um array com 10 números e percorrer o array utilizando for. Somar todo os números e ao final da execução do for, imprimir o resultado da soma.
?

// Item 11: Criar um array com 10 números e percorrer o array utilizando o for of. Filtrar todos os números menores que 4 e criar um novo array com os números encontrados. Imprimir o array com os números encontrados.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

for (let number of array) {
	console.log(String(number))
}

// Item 12: Criar um array com 10 números e percorrer o array utilizando o for of. Imprimir todos os números do array dentro do for of.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

let resultado = 0

for (let i = 0; i < array.lenght; i++) {
	resultado += array[i]
}

console.log(resultado)

// Item 13: Criar um array com 10 números e percorrer o array utilizando o for of. Imprimir a todos os números do array multiplicado por 2. Exemplo: n * 2 (n representa cada número do array) dentro do for of.
?

// Item 14: Criar um array com 10 números e percorrer o array utilizando o for of. Imprimir a todos os números do array multiplicado por 2. Exemplo: n * 2 (n representa cada número do array) dentro do for of.
?

// Item 15: Criar um array com 10 números e percorrer o array utilziando for of. Somar todos os números e ao final de execução do for of, imprimir o resultado da soma.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

let resultado = 0

for (let number of array) {
	resultado += number
}

console.log(resultado)

// Item 16: Criar um array com 10 números e percorrer o array utilizando for of. Filtrar todos os números menores que 4 e criar um novo array com os números enontrados. Imprimir o array com os números filtrados.
// Primeira forma de se resolver
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
const filteredArray = [];

for (let i = 0; i < array.length; i++) {
	const number = array[i]

	if (number > 4) {
	filteredArray.push(number);
	}
}

console.log(filteredArray)

// Segunda forma de se resolver
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
const filteredArray = [];

for (let number of array) {
	if (number > 4) {
		 filteredArray.push(number)
	}
}

console.log(filteredArray)

```

#### Exercício de Arrays - map

```js

// Item 17: Criar um array com 10 números e percorrer o array utilizando map. Multiplicar cada item por 2. Imprimir o novo array gerado ao fim da execução.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

console.log(array.map(item => item * 2))

// Item 18: Criar um array com 10 números e percorrer o array utilizando map. Transformar todos os itens do array em string e imprimir o novo array gerado ao fim da execução.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
// Resolvendo de uma forma
console.log(array.map(item => String (item)))

const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
// Resolvendo de outra forma
console.log(array.map(item => `${item}`))

```

#### Exercício de Arrays - filter

```js

// Item 19: Criar um array com 10 números e percorrer o array utilizando o filter. Filtrar todos os números menores que 4 e imprimir o novo array gerado ao fim da execução.
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

console.log(array.filter(item => item > 4))

```

#### Exercício de Arrays - reduce

```js

// Item 20: Criar um array com 10 números e percorrer o array utilizando o reduce. Somos todos os números e ao final da execução do reduce, imprimir o resultado de soma. 
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

console.log(array.reduce((acumulador, item) => acumulador + item))

```

#### Exercício de Arrays - forEach

```js

// Item 21: Criar um array com 10 números e percorrer o array utilizando forEach, imprimir todos os números do array dentro do forEach. 
?

// Item 22: Criar um array com 10 números e percorrer o array utilizando forEach, imprimir a todos os números do array multiplicado por 2. Exemplo: n * 2 (n representa cada número do array) dentro do forEach.
?

// Item 23: Criar um array com 10 números e percorrer o array utilizando o forEach. Transformar todos os itens do array em string e imprimir todos os números do array dentro do forEach.
?

// Item 24: Criar um array com 10 números e percorrer o array utilizando forEach. Somar todo os números e ao final de execução do forEach, imprimir o resultado de soma.
?

// Item 25: Criar um array com 10 números e percorrer o array utilizando o forEach. Filtrar todos os números menores que 4 e criar um novo array com os números encontrados. Imprimir o array com os números filtrados
?

```