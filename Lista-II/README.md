# Lista de Exercícios II

> À partir do dia 28 de janeiro. Laços de repetição e function são os assuntos que norteiam essa atividade. 

```js

// Escreva o trecho de código para: A partir do valor da variável numero, se o valor for 1, o console imprime "1"; se for 2, o console imprime "2"; se for 3, imprime "3"; se for diferente desses valores, imprime "Não é um número esperado".
var numero = parseInt(prompt('Insira um valor para a base:'));
switch (numero) {
  case 1:
  case 2:
  case 3:
    console.log(numero);
  break;
  default:
    console.log('Não é um número esperado');
}

function numero(entrada){if ( entrada == 1 || entrada == 2 || entrada == 3){console.log(entrada);} else {console.log('Não é um número esperado')}}

// A partir do valor da variável contagemRegressiva, se o valor for 1, o console imprime "1"; se for 2, o console imprime "2\n1"; se for 3, imprime "3\n2\n1"; se for diferente desses valores, imprime "Não sei contar além do 3".
function numero (contagemRegressiva){
( contagemRegressiva == 1 ) ?
  console.log("1") :
( contagemRegressiva == 2 ) ?
  console.log("2\n1") :
( contagemRegressiva == 3 ) ?
  console.log("3\n2\n1") :
  console.log("Não sei contar além do 3")
}

// Escreva o trecho de código para: o console imprime na tela a string "Olá" cinco vezes.
function mensagem () {
for ( var i = 0; i < 5; i++ ) {
  console.log("Olá")
  }
}

console.log("Olá\nOlá\nOlá\nOlá\nOlá")

console.log('Olá\n'.repeat(5))

// Escreva o trecho de código para: o console imprime na tela números de 1 até o limite armazenado na variável limite, incluindo esse valor, cada número em uma linha.
var limite = parseInt(prompt('Insira um valor limite: '));
for ( i = 1; i <= limite ; i++ ) {
  console.log(limite)
}

// Escreva o trecho de código para:O console pergunta para o usuário, através do prompt, "Qual é o seu nome?" e continua perguntando até que o usuário responda com algo diferente de só apertar ok ou cancelar, sem escrever nada.
function mensagem () {
var usuario = prompt('Qual é seu nome?');
if ( usuario === '' || usuario === undefined ) {
  console.log("Erro");
  mensagem()
} else {
  return
  }
}

do {
  entrada = prompt("Qual é o seu nome?")
} while(entrada === null || entrada === "")

// Escreva o trecho de código para: crie um loop infinito (Não execute o código). Explique o porquê de o loop ser infinito.
for ( var i; ; i++ ) {console.log(i)}

for(;;;){console.log('loop')}

while(true){console.log('loop)}

while(true){console.log('loop)}

// Escreva uma função, com o nome inutil, que não recebe nenhum parâmetro, não executa nenhum processamento, não imprime nenhum texto no console e não retorna nenhum valor.
function inutil() {
}

// Dada a função soma: function soma(n1, n2){return n1 + n2;}Qual é a diferença entre executar o comando: resultado = soma e executar o comando: resultado = soma(1, 2).
O comando  resultado = soma atribui a função soma à variável resultado (uma vez que deve estar previamente declarada), já o comando resultado = soma(1, 2) atribui à variável resultado o valor de n1 e n2 determinado pelo usuário que está contido dentro da função. 

// Escreva uma função, com o nome papagaio, que tem o parâmetro texto, uma string, e imprime no console essa string, sem retornar nenhum valor. Depois, escreva o comando que executa a função com o valor do parâmetro texto: "Eu não sou um papagaio!".
function papagaio( texto ) {
   console.log(texto)
}
papagaio('Eu não sou um papagaio')

// Escreva uma função, com o nome positivista, que sempre retorne o valor booleano true. Depois, escreva o comando que executa essa função.
function positivista () {
  return true
}

positivista ()

// Escreva uma função que receba um valor numérico com entrada (não precisa testar se é numérico), faça algum processamento com esse valor, e retorne o resultado desse processamento. Depois, escreva o comando que armazena o retorno da função na variável resultado e use como valor de entrada o número 3,5.
function ENumerico ( numero, resultado ) {
  resultado = numero * numero
  return resultado
}

resultado = ENumerico(3.5,0)

// Escreva uma função, com o nome manda, que tem como parâmetros funcao, uma função, e valor, um valor de qualquer tipo. A função manda deve executar a funcao com o valor como argumento e retornar o que for retornado pela funcao. Depois, escreva o comando que executa a função manda com a função da pergunta anterior, como argumento da funcao, e o valor 1, como argumento do valor.
function manda ( funcao, valor ) {
  return funcao ( valor )
}

manda ( ENumerico, 1 )

// Considere uma variável x com o valor 5. Escreva uma função, com o nome mudaX, que altere o valor de x para 10. Escreva o comando que executa essa função. Depois da execução da função, qual é o valor armazenado em x?
x = 5

function mudaX () {
  x = 10
  return x
}

mudaX()

// Considere uma variável x com o valor 5. Escreva uma função, com o nome escopoX, que não tem nenhum parâmetro e não retorna nenhum valor. Dentro da função declare x e atribua o valor 10. Escreva o comando que executa essa função. Depois da execução da função, qual é o valor armazenado em x?
x = 5

function escopoX () {
  var x = 10
}

escopoX()
// X retorna 5, pois a declaração 'x=10' não faz parte do escopo global do código

```
