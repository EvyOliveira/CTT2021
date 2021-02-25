# Lista de Exercícios da Apostila CTT 2021

> Engloba todo o conteúdo do módulo de Linguagem de Programação.

```js

// Escreva uma função chamada diferenca que retorne a diferença de dois números. 
?

// Escreva uma função que retorne o quadrado de um número.
function quadrado(base) {
  var base = parseInt(prompt('Insira um valor para a base:'));
  return base ** 2;
}

// Escreva uma função que retorne a raiz quadrada de um número.
function raizQuadrada(num) {
  var num = parseInt(prompt('Insira um valor para ser calculada a raiz quadrada:'));
  return Math. sqrt(num);
}

// Escreva uma função que, dada uma lista de numeros inteiros, retorne o menor número.
function buscaMenor(array){
  var menor = array[0];
  console.log('Declarei menor com o valor'+menor);
  for( var posicao = 0; posicao < array.length; posicao++){
    console.log('Vamos ver se o numero '+array[posicao]+' da posicao '+posicao+' é menor do que '+menor)
      if( array[posicao] < menor){
        console.log('É menor')
        menor = array[posicao];
        console.log('Atribuí '+menor+' à variável menor')
      } else {
        console.log('Não é menor');
      }
  }
  console.log('Vou retornar menor com o valor '+menor)
  return menor;
}

// Escreva uma função que, dada uma lista de numeros inteiros, retorne o maior número.
var array = [ -1, -3, 0, 9, -7, 6, 2, 0];
function buscaMaior(array){
  var maior = array[0];
  console.log(' Declarei maior com o valor '+ maior);
    for( var posicao = 0; posicao < array.length; posicao++ ){
      console.log(' Vamos ver se o número '+ array[posicao] +' da posicao '+ posicao + ' é maior do que ' + maior)
        if( array[posicao] > maior ){
          console.log(' É maior. ');
          maior = array[posicao];
          console.log(' Atribui '+ maior +' à variável maior. ');
        } else {
          console.log(' Não é maior. ');
        }
    }
  console.log(' Vou retornar o maior valor com o valor '+ maior );
  return menor;
}

buscaMaior(array)

// Escreva uma função que, dada uma lista de numeros inteiros, retorne a soma.
?

// Escreva uma função que, dados os três lados de um triângulo, calcula o seu perímetro.
function perimetroTri(){
  var a = parseInt(prompt('Insira um valor para o lado A do triângulo'));
  var b = parseInt(prompt('Insira um valor para o lado B do triângulo'));
  var c = parseInt(prompt('Insira um valor para o lado C do triângulo'));
  return a + b + c;
}

// Escreva uma função que, dado o raio de um círculo, calcule a sua área. Considere pi = 22/7.
function calcArea(raio){
  var raio = parseInt(prompt('Insira um valor para o raio'));
  return 22/7 * (raio ** 2);
}

// Escreva uma função que, dada uma String, imprima essa String ao contrário. Considere as funções chartAt de String e a lógica abaixo:
function inverter(vetor){
  console.log('Criei um array vazio');
  resultado = [];
  console.log('Criei a variavel posicao que recebeu o valor '+vetor.length-1);
  posicao = vetor.length - 1;
  console.log('Enquanto posicao for maior ou igual a 0')
    while ( posicao >= 0 ){
      console.log('Adiciono ao resultado o valor '+vetor[posicao]+' presente na posicao '+posicao)
      resultado.push(vetor[posicao]);
      console.log('Subtraio um de posicao resultado em '+posicao-1)
posicao--;
}
  console.log("Retorno o resultado com "+resultado)
  return resultado;
}

string_resultado = resultado.join(‘’)

// Escreva uma função que, dados dia, mês e ano, calcula quantos dias faltam para o próximo natal.
?

// Escreva uma função que converta graus Farenheit para Celsius. Considere que (F − 32) × 5/9 = C.
function temp_fah (f) {
  return (f - 32) * 5/9;
}; 

temp_fah();

// Escreva uma função que converta graus Celsius para Farenheit. Considere que (F − 32) × 5/9 = C.
function temp_cel (c) {
  return (c * 1.8 + 32);
};

temp_cel();

// Escreva uma função que verifica se um ano é bissexto. Considere que anos múltiplos de 4 e que não sejam múltiplos de 100 são bissextos. 
function bissexto (ano) {
  ( ( ano % 4 == 0) && (ano % 100 == 0)) ?
  (ano % 400 == 0) ? console.log('O ano ' + ano + ' é bissexto') : console.log('O ano ' + ano + ' não é bissexto') :
  console.log('O ano não é bissexto');
}

// Escreva uma função que, dados dia, mês e ano, calcula quantos dias do ano se passaram até essa data. Exemplo: dia 02/02/2021 será o dia 33 do ano.
?

// Escreva uma função que valide se uma string é um palíndromo.
?

/* Crie um objeto chamado calculadora, com as funções:
soma(numero1, numero2) que retorna a soma dos dois números;
diferenca(numero1, numero2) que retorna a diferença dos dois números;
multiplicacao(numero1, numero2) que retorna a multiplicação dos dois números;
divisao(numero1, numero2) que retorna a divisão dos dois números. Execute as quatro operações a partir desse objeto. */
Calculadora = {
  soma: function( numero1, numero2 ){
  return numero1 + numero2;
},
  diferenca: function( numero1, numero2 ){
  return numero1 - numero2;
},
  multiplicacao: function( numero1, numero2 ){
  return numero1 * numero2;
},
  divisao: function( numero1, numero2 ){
  return numero1 / numero2;
}

// Crie uma funcao que, dado um numero entre 0 e 9, informa se ele é par ou impar. Use como referência o código abaixo:
function ePar(numero){
  switch (numero) {
    case 0:
    case 2:
    case 4:
    case 6:
    case 8:
      console.log('É par);
      break;
    case 1:
    case 3:
    case 5:
    case 7:
    case 9:
      console.log('É impar);
      break;
    default:
      console.log('Nao conheco');
  }
}

```