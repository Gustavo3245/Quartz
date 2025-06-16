---
tags:
  - ComputerScience
Datatime: 05/08/2024
Conteúdo: Valores e operações booleanas, portas AND, OR, NOT e etc.
---
# Boolean Logic

### Álgebra Booleana

é um ramo da matemática que generaliza a aritmética.serve para testar e comprovar conceitos e operações (adição,subtração,multiplicação e divisão).

Na Álgebra de Boole existem apenas três operadores E, OU e NÃO (AND, OR, NOT). Estas três funções são as únicas operações necessárias para efetuar comparações ou as quatro operações aritméticas base.

1. Diferente da álgebra comum, são usados nos lugares dos números, os valores True and False, que representa respectivamente a passagem de eletricidade e a não passagem da mesma.

2. As operações também são diferentes, operações de soma, substração e outras não são utilizadas na álgebra booleana,

Atualmente todos os computadores usam a Álgebra de Boole materializada em microchips que contêm milhares de interruptores miniaturizados combinados em portas (gates) lógicos que produzem os resultados das operações utilizando uma linguagem binária.

Transistor Básico.

![[Pasted image 20240805143639.png]]


Existem 7 blocos lógicos.

Os blocos lógicos são divididos em 7 classes:

- [E (AND)](https://pt.wikipedia.org/wiki/E_(AND) "E (AND)")
- [OU (OR)](https://pt.wikipedia.org/wiki/OU_(OR) "OU (OR)")
- [NÃO (NOT)](https://pt.wikipedia.org/wiki/N%C3%83O_(NOT) "NÃO (NOT)")
- [NE (NAND)](https://pt.wikipedia.org/wiki/NE_(NAND) "NE (NAND)")
- [NOU (NOR)](https://pt.wikipedia.org/wiki/NOU_(NOR) "NOU (NOR)")
- [OU EXCLUSIVO (XOR)](https://pt.wikipedia.org/wiki/XOR "XOR")
- [NÃO-OU EXCLUSIVO (XNOR)](https://pt.wikipedia.org/wiki/Porta_XNOR "Porta XNOR")

1. Porta AND, a saída é verdade apenas quando ambas as entradas são verdadeiras. 

	![[Pasted image 20240805144316.png]]


2. Porta OR, a saída é verdade quando uma ou as duas entradas são verdadeiras.

	![[Pasted image 20240805144440.png]]


3. Porta NOT, recebe apenas uma entrada, inverte o valor de entrada.

	![[Pasted image 20240805144148.png]]


4. Porta NAND, porta AND + NOT, inverte os valores da porta AND.

	

5. Porta NOR, Porta OR + NOT, inverte os valores da porta OR. 

	

6.  porta XOR, essa porta retorna true quando as entradas são valores diferentes.

	

7. porta XNOR, inverte os valores da porta XOR.