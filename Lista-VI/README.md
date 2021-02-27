# Lista de Exercícios VI

> À partir do dia 26 de fevereiro. Exercícios sobre funções assíncronas com callback.

```js

// Criar uma function chamada print que recebe uma string por parâmetro e que imprima a string passada por parâmetro. Criar uma função que receba uma string e a função print por parâmetro e execute a função de callback para imprimir a string recebida.
function print (s) {
  console.log(s)
}

function imprimeComCallbacks(s, callbackFn) {
  const uppercase = s.toUpperCase()
  callbackFn(uppercase)
}

imprimeComCallbacks('Olá callback', print)

// Criar uma function chamada soma que recebe dois números por parâmetro [n1, n2] e retorna a soma dos dois números. Criar uma função chamada executaSoma1 que recebe um número e a função soma por parâmetro, executa a função soma passando o número [n] por parâmetro para a função soma sendo n -> n1, n -> n2, guardar o valor de retorno da função na variável const resultado. Criar uma cópia da função executaSoma1, nomeando-a como executaSoma2. A função executaSoma2 deve ser executada ao final do bloco da função executaSoma1, recebendo por parâmetro a variável resultado e a função soma. Imprimir a variável resultado a cada execução de soma.
const soma = (n1, n2) => n1 + n2

const executaSoma2 = (n, callbackFn2) => {
  const resultado = callbackFn2(n, n)
  console.log('resultado executaSoma2 ==> ', resultado)
  return resultado
}

const executaSoma1 = (n, callbackFn1) => {
  console.log('executaSoma1', n, callbackFn1)
  const resultado = callbackFn1(n, n)
  console.log('resultado executaSoma ==> ', resultado)
  return executaSoma2(resultado, soma)
}

console.log(executaSoma1(1, soma))

```