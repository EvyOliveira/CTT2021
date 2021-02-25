# Lista de Exercícios I

> 21 de janeiro ao dia 26 de janeiro. Aborda conteúdos desde variáveis, atribuição, operações matemáticas e lógicas, Infinity até objetos customizados.

```js

// Declare uma variavel com o nome variável.
var variavel;

// Qual é o valor da var variavel ?
undefined

// Atribua como o valor da variavel o valor 3.
variavel = 3;

// Declare e atribua a variavel saudação a string boa noite.
var saudacao = 'Boa noite!';

// Declare a variável booleano e atribua um valor booleano.
var booleano = true;

// Sem declarar a variável numero, atribuir a ela o número dois e meio.
= 2.5

// Altere o valor da variável numero para a string "número".
numero = 'numero';

// Escreva o comando para imprimir no console as frases:
// Campinas Tech Talents
// Trilha Sensedia - NodeJS
function pulaLinha() {
  document.write("<br>");
}

console.log('Campinas Tech Talents</br>Trilha Sensedia - NodeJS');

console.log('Campinas Tech Talents\nTrilha Sensedia - NodeJS');

console.log('Campinas Tech Talents');
console.log('Trilha Sensedia - NodeJS');

// Escreva o comando para imprimir no console o valor da variável texto.
console.log(texto);

// Escreva uma expressão de soma de dois números, que você pode escolher.
num1 + num2;

// Atribua a uma variável de sua escolha o resultado da subtração de dois números, que você pode escolher.
sub = 10 - 4

// Declare e atribua à variável produto o resultado da multiplicação de dois números, que você pode escolher.
var produto = 100 * 100;

// Escreva uma expressão de divisão de dois números que resulte em um número não inteiro.
15 / 16;

// Atribua a uma variável de sua escolha o resultado de uma divisão que resulte em Infinity.
resultado = 1 / 0

// Declare e atribua à variável resto o resto da divisão de 2021 por 11.
var resto = 2021 % 11;

// Escreva o resultado de 2 elevado à 20ª potência - 2 ** 20.
1048576

// Atribua à variável futuro o valor 2021. Some o valor 10 ao valor de futuro e atribua o resultado a essa mesma variável.
futuro = 2021;
futuro += 10;

// Declare e atribua à variável tempoParaAcabar o valor 60 e, em seguida, decremente (subtraia 1) do valor dessa variável.
var tempoParaAcabar = 60;
tempoParaAcabar-= 1;

// Escreva uma expressão comparando se 3 é maior que 5 e diga qual é o resultado retornado.
console.log(3 > 5);
false

// Atribua à variável menorIgual o resultado da comparação se -1 é menor ou igual a -5.
menorIgual = -1 <= -5

// Escreva uma expressão que compare se o conteúdo da variável entrada é igual ao da variável esperado, desconsiderando o tipo.
entrada == esperado;

// Escreva uma expressão que compare se o número 2 é igual à string "2", considerando o tipo, e diga qual é o resultado retornado.
console.log(2 === '2');

// Escreva uma expressão que compare se o booleano true é diferente da string "true", considerando o tipo, e diga qual é o resultado retornado.
console.log(true !== 'true');

// Atribua à variável vaiChover o resultado da operação lógica OU entre as variáveis temNuvemNoCeu e laveiCarro.
vaiChover = temNuvemNoCeu || laveiCarro;

// Escreva uma expressão que realize a operação lógica E entre as variáveis fome e sono.
fome && sono;

// Escreva o trecho de código para:
// Se o valor da variável imprime for true, o console imprime na tela a string "imprimi".
if( var imprime == true ) {
  console.log('Imprimi');
}

// Escreva o trecho de código para:
// Se o valor da variável x for maior ou igual a 5, o console imprime na tela a string "maior ou igual a 5". Caso contrário, imprime "menor que 5".
if( x >= 5) {
  console.log('Maior ou igual a 5');
 } else {
  console.log('Menor que 5');
};

// Se o valor da variável numero for um número, o código retorna true. Caso contrário, retorna false.
typeof num == 'number' ? true : false

// Escreva o trecho de código para:
// Se o valor da variável idade for menor que 12, o console imprime na tela a string "criança". Se o valor da variável idade for maior ou igual a 12 e menor que 18, o console imprime na tela a string "adolescente". Se o valor da variável idade for maior ou igual a 18, o console imprime na tela a string "adulto".
if(idade < 12) {
  console.log("Criança");
 } else {
if (idade >= 12 ?? idade < 18) {
  console.log("Adolescente");
} else {
 console.log("Adulto");
  }
}

// Objeto customizado para validação de dia, mês e ano, considerando os anos bissextos.
Data = {
  ano: undefined,
  mes: undefined,
  dia: undefined,
  setAno: function(entrada){
     if( this.validaAno(entrada) ){
        this.ano = entrada;
        this.mes = undefined;
        this.dia = undefined;
        alert('Variavel ano recebeu o valor '+entrada);
     } else {
        alert('Variavel entrada tem valor inválido '+entrada);
     }
  },
  setMes: function(entrada){
     if( this.validaMes(entrada) ){
        this.mes = entrada;
        this.dia = undefined;
        alert('Variavel mes recebeu o valor '+entrada);
     } else {
        alert('Variavel entrada tem valor inválido '+entrada);
     }
  },
  setDia: function(entrada){
     if( this.validaDia(entrada) ){
        this.dia = entrada;
        alert('Variavel dia recebeu o valor '+entrada);
     } else {
        alert('Variavel entrada tem valor inválido '+entrada);
     }
  },
  validaAno: function(entrada){
     return this.validaInteiro(entrada)
  },
  validaMes: function(entrada){
     return entrada > 0 && entrada < 13 && this.validaInteiro(entrada);
  },
  validaDia: function(entrada){
     return entrada > 0 && entrada <= this.getQuantidadeDiasDoMes(this.ano, this.mes) && this.validaInteiro(entrada);
  },
  validaInteiro: function(entrada){
     return Number.isInteger(entrada)
  },
  getQuantidadeDiasDoMes: function(ano, mes){
    switch (mes){
        case 1:
        case 3:
        case 5:
        case 7:
        case 8:
        case 10:
        case 12:
             return 31;
        case 4:
        case 6:
        case 9:
        case 11:
             return 30;
        case 2:
             if( this.isBissexto(ano) ){
                 return 29
             }
             return 28;
        default:
             return undefined;
    }
  },
  isBissexto: function(ano){
    return ( ano % 400 === 0 || (( ano % 4 === 0 && ano % 100 !== 0 )));
  }
}

// Saída desse valor é false
Data.validaFormatoAno(1.5)
// Saída desse valor é true
Data.validaFormatoAno(2020)
// Saída desse valor é false
Data.validaMes(13)
// Saída desse valor é true
Data.validaMes(1)
// Saída desse valor é false
Data.isBissexto(1700);
// Saída desse valor é true
Data.isBissexto(2000);

// Objeto customizado para validação do CPF.
function isNumerico(entrada) {
   var temDigitoNaoNumerico = false;
   console.log('Tamanho da entrada: '+entrada.length)
   for(let i = 0; i < entrada.length; i++){
   console.log('Para o caracter ' + entrada.charAt(i)+' da posição '+ i)
   switch(entrada.charAt(i)){
       case '0':
       case '1':
       case '2':
       case '3':
       case '4':
       case '5':
       case '6':
       case '7':
       case '8':
       case '9':
       break;
       default:
           temDigitoNaoNumerico = true;
       }
   }
   return !temdigitoNaoNumerico;
};

function validaCpf(cpfString){
if( cpfString.length != 11 ){
   console.log("A entrada deve ter 11 caracteres. Tamanho da entrada: " + cpfString.length);
   return false;
}
if( !isNumerico(cpfString) ){
   console.log('A entrada deve ser exclusivamente numérica');
   return false;
}
let somaPrimeiroDigitoVerificador = 0;
for(let i = 0; i < 9; i++){
   somaPrimeiroDigitoVerificador += (cpfString.charAt(i) * (10 - i)
}
primeiroDigitoVerificador = (somaPrimeiroDigitoVerificador * 10 ) % 11;
if( primeiroDigitoVerificador == 10 ) {
   primeiroDigitoVerificador = 0;
};
let somaSegundodigitoVerificador = 0;
for(let i = 0; i < 10; 1++) {
   somaSegundoDigitoVerificador += ( cpfString.charAt(i) * (11 -i) )
}
segundoDigitoVerificador = (somaSegundoDigitoVerificador * 10 ) % 11;
if( segundoDigitoVerificador == 10) {
   segundoDigitoVerificador = 0;
}
   return cpfString.charAt(9) == primeiroDigitoVerificador && cpfString.charAt(10) == segundoDigitoVerificador;

}

// Código tratando sobre a data de nascimento do usuário utilizando getters e setters.
var usuario = {
  nome: '',
  ano_nascimento: 0,
  mes_nascimento: 0,
  dia_nascimento: 0,
  // objetivo: validar data de nascimento
  set_nome: function () {
      nome_prompt = prompt('Qual é seu nome?')
      // validação do nome
      if( nome_prompt === '' || nome_prompt === undefined){  
          nome_prompt = prompt('Qual é seu nome?')
      } else {
          this.nome = nome_prompt
      }
  set_ano_nascimento: function () {
      ano_prompt = prompt('Qual é o ano do seu nascimento?')
      // validação do ano
      while( ano_prompt == '' || ano_prompt <= 0){  
          ano_prompt = prompt('Qual é o ano do seu nascimento?')
      } else {
          this.ano = ano_prompt
      }
  }
  set_mes_nascimento: function(){
      mes_prompt = prompt('Qual é o mês do seu nascimento?')
      // validação do ano
      while( mes_prompt == '' || mes_prompt <= 0 || mes_prompt > 12){  
          ano_prompt = prompt('Por favor, insira um valor entre 1 e 12')
      } else {
          this.ano = ano_prompt
      }
  }
    set_dia_nascimento: function(){
      dia_prompt = prompt("Qual é o dia do seu nascimento?");
      // Validação do dia
      this.dia_nascimento = dia_prompt;
  }
  get_nome: function {
      if (this.nome === '') {
          this.set_nome
      } else {
          return this.nome
      }
  }
  get_ano_nascimento: function() {
      return this.ano_nascimento
  }
  get_mes_nascimento: function(){
      if (1 <= this.mes_nascimento <= 12 ) {
          return this.mes_nascimento;
      } else {
          this.set_mes_nascimento
      }
  }
  get_dia_nascimento: function(){
      return this.dia_nascimento;
  get_data_nascimento: function() {
      this.get_ano_nascimento
  }
  }
}


```
