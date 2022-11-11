# Trabalho em Assembly
Realizado na disciplina de Organização de Computadores, ministrada pelo professor Ricardo Ferreira
Ana Laura Tavares
Barbara Cristina Fonseca
Gabriela Ouriques
Lara Fernandes Pereira
Maria Victoria Fernandes Vaz
<br><br>

#### 1. Fazer a multiplicação de float 7 bits
 * Entrada: 2 números em binário com float nos registradores t0 e t1. Exemplo t0= ...011 1000, t1=...100 0110
 * Saida: Resultado da Multiplicação no registrador t2.
 * Adicione comentarios no seu código e se possível um pseudo código com o algoritmo
 ```
 addi t0,x0,0x38
 addi t1,x0,0x46
 # Adicionar seu código
 # resultado estará em t2
 ```
 
 #### 2. Fazer um printf 2^e * 1.x onde e=-3 a +4 e x é parte fracionária
 * imprimir a resposta usando caracteres ASCII
 * Entrada valor em t0
 * Saida será em ASCII na memoria a partir da posicao GP, primeiro o expoente, depois o numero. Por exemplo 011 1000 = 2^3-3*(1+1/2) = 2^0 * 1.5.
 ```
0x1000000c				
0x10000008	5
0x10000004	1 .
0x10000000	2 ^ 0  
 ```
 #### 3. Algoritmo KNN com duas dimensões
 
 ![](https://miro.medium.com/max/1024/1*CcnlWd_JbbAiO5J0WYdaqw.png)
 
 * Entrada : O vetor terá duas dimensões e será armazenado a partir da posição GP. Primeiro tem o valor de K, depois seu ponto X,Y, seguido pelo vetor que terminar com -1.
 * Saida: Irá ser escrita em GP, sobreescrevendo o valor de k. Pode ter três classes: 0, 1, 2;
 ```
 Memoria = 3, 2,1,  0, 0, 1  , 0, 1, 2 ,   1,0, 1 ,  2,0,1,  3,0,1,   0,2, 2,  0,3, 2  -1
 então K=3, queremos classificar o ponto (2,1) 
 a resposta será classe 1. 
 ```
 [link para o exemplo](https://excalidraw.com/#json=jCg-UmaMlxfYCTQMU6qVm,BhUYn8dzWb3wTNhh0yVZvA)

 
