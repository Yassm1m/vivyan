# vivyan
tipos de dados, estrutura condicional e estrutura de repetição de linguagem Java 

ESTRUTURA CONDICIONAL-

*estrutura condicional simples (se - if)*

a estrutura condicional é baseada em uma condicao que se for atendendida o algoritmo toma uma descisão. exemplo: 

SE (A > B)ENTAO 
 escreva("o numero A é maior que o numero B")
FIMSE 

Agora se pensar na linguagem C o algoritmo mudara e seguira a segunte forma, exemplo:

if(a > b){
   printf("o numero %d maior que o numero %d", a, b);
}

uma pequena observacao  utilizando a linguagem C , o fundamento das estruturas condicionais são os mesmos para qualquer linguagem 
somente  alterando a sintaxe  particular de cada uma .



*estruturas condicional composta (senao - else)*

a diferença de uma condicional simples para uma composta, é que nesse caso mesmo se  a condiçao for FALSA nosso algoritmo 
tambem 
ira ter uma execuçao e seguira o programa. exemplo : 

se(A > B)ENTAO 
  exibir mensagem "o numero A e maior que o numero B"
  SENAO
  exibir mensagem "o numero A é menor que o numero B"
  
utilizando a linguagem C, o algoritmo ficara da seguinte maneira 

 if (A > B) {
    printf("o número %d é maior que o número %d", a, b);
} else {
    printf("o número %d é menor que o número %d", a, b);
}

Note que o código acima representa a seguinte condição: se o número A for maior que o número B, o algoritmo irá entender que 
a condição é verdadeira e deve exibir a mensagem “o número A é maior que o número B”, se esta condição não for atendida, ou 
seja, se ela for falsa.
Diferente do exemplo sobre estrutura condicional simples onde o algoritmo não tomava nenhuma ação, aqui ele toma uma decisão 
diferente, exibindo a mensagem “o número A é menor que o número B”.

*ESTRUTURAS DE REPETICAO*

para situacoes no qual precisamos executar a mesma tarefa mais de uma vez podemos utilizar a estrutura de repeticao dentro delas existem 3 estruturas, sendo elas enquanto(while), para(for) e 


*enquanto(while)*

Uma das condições que podemos usar é o enquanto, ou seja, enquanto a expressão booleana for verdadeira o algoritmo executa o 
bloco proposto, por fim é necessário que algo dentro do bloco altere a condição.
Podemos exemplificar o uso do enquanto supondo um algoritmo que retorne o resultado de uma tabuada, onde:

i sendo uma variável inteira de valor 1.

exemplo : 
i=1
escreva("digite o numero da tabuada")
 ENQUANTO (i <= 10)faca
	 result:= numtabuada * i
 	 i:= i+1 
    escreva ("o resultado é: ", result)
FIM DA CONDIÇÃO

ja na linguagem C ficaria da seguinte maneira :

while (i <= 10) {
       printf("9 x %d = %d\n", i, 9 * i);
       i++;
   }

a condicao que colocamos no algoritmo é de que a variavel 'i' ira repetir o programa ate que seja igual a 10. Enquanto isso sera exibido a mensagem "9 x i =(9*i)". a cada linha executada sera somado a variavel i que é igual a 1. essa soma é chamada de iteraçao, e muitos programadores referencia-se a ela como i++. quando i chegar ao valor de 11 o algoritmo ira parar de executar a soma e desta forma o resultado ira aparecer na tela


*para(for)*

a condiçao PARA  tem a mesma intencao que a ENQUANTO, 
porem ela é mais utilizado quando se sabe a quantidade de 
vezes que ira se repetir, como listar os valores de um 
vetor por exemplo. tambem vale ressaltar a legibilidade do 
codigo mais limpo, seguindo o mesmo exemplo da tabuada 
citado a cima temos um exemplo: 

escreva ("digite a tabuada: ")
leia(numtabuada)
 para i de 1 ate 10 passa 1 faca
  result:= numtabuada * i 
   i:= i +1
   escreva ("o numero da tabuada é: "result)
  fimpara
 fimalgoritmo 
 
 
 na linguagem C fica da seguinte maneira :
 
 for (int i = 1; i <= 10; i++) {
       printf("9 x %d = %d\n", i, 9 * i);
   }



Note que ao usar o PARA (for) o contador (a variável i) é inicializado e incrementado na própria condição do laço junto a expressão booleana a ser atendida, deixando o código mais limpo e sem a necessidade de criar variáveis adicionais.
No fim o retorno aguardado será o mesmo que do exemplo que utilizamos a do laço enquanto.



*estrutura repita- ate*

A estrutura de repetição Repita-até é utilizada quando
um conjunto de comandos deve ser executado
repetidamente, até que uma condição (expressão lógica)
seja verdadeira. ▫ O comando é executado uma vez.
▫ Após, a condição é testada: se ela for falsa, a lista de
comandos é executada novamente e este processo é
repetido até que a condição seja verdadeira, quando
então a execução prossegue pelo comando
imediatamente seguinte ao final da construção, exemplo:

numtabuada,result:real
i:inteiro

inicio
  i=1
  escreva ("digite o numero da tabuada: ")
  leia(numtabuada)
   repita 
    result:= numtabuada*i 
    i:= 1+1 
     screva("o resultado é : ", result)
   ate(i > 10)
fimalgoritmo 





TIPOS DE DADOS NA  LINGUAGEM JAVA*

Em Java, existem vários tipos de dados, que podem ser divididos em dois grupos principais: tipos de dados primitivos e tipos de dados de referência.

Os tipos de dados primitivos são tipos básicos, que representam valores simples, como números e caracteres. Os tipos de dados primitivos incluem:

.boolean: representa um valor verdadeiro ou falso (true ou false)
.byte: representa um número inteiro de 8 bits, com sinal
.short: representa um número inteiro de 16 bits, com sinal
.int: representa um número inteiro de 32 bits, com sinal
.long: representa um número inteiro de 64 bits, com sinal
.float: representa um número de ponto flutuante de 32 bits
.double: representa um número de ponto flutuante de 64 bits
.char: representa um caractere Unicode de 16 bits
Os tipos de dados de referência são tipos que representam objetos em Java, incluindo strings, arrays e objetos definidos pelo usuário. Alguns exemplos de tipos de dados de referência incluem:

.String: representa uma sequência de caracteres
.Array: representa uma coleção de elementos do mesmo tipo de dados
.Classe: representa um tipo de dados definido pelo usuário
.Interface: define um conjunto de métodos que uma classe pode implementar


