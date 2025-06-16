---
tags:
  - ComputerScience
Datatime: 06/08/2024
Conteúdo: Como os computadores calculam, como eles realizam funções e tudo mais.
Linked:
  - "[[Binary]]"
  - "[[Boolean,Gates Logic]]"
---
## (ULA) unidade lógica e aritmética
a ULA, é um circuito digital que realiza operações de adição e booleana.A ULA é uma peça fundamental da unidade central de processamento (UCP), e de todos os processadores.

A ULA executa as principais operações lógicas e aritméticas do computador. Ela soma, subtrai, divide, determina se um número é positivo ou negativo ou se é zero. Além de executar funções aritméticas, uma ULA deve ser capaz de determinar se uma quantidade é menor ou maior que outra e quando quantidades são iguais. A ULA pode executar funções lógicas com letras e com números.

1. Muitas das ações dos computadores são executadas pela ULA. Esta recebe dados dos [registradores](https://pt.wikipedia.org/wiki/Registradores "Registradores"), que são processados e os resultados da operação são armazenados nos registradores de saída. Outros mecanismos movem os dados entre esses registradores e a memória.

2. *Uma unidade de controle controla a ULA, através de circuitos que dizem que operações a ULA deve realizar.*

### Opções de ULAs para cálculos. (Realizar uma Raiz Quadrada).

![[Pasted image 20240806132519.png]]

### Half Adder
Meio somador é um circuito que possui a capacidade de somar dois números binários.

1. ele funciona em forma de um portão lógico **AND** e **XOR**,tendo dois valores de entrada(dois bits), e dois valores de saída.

2. O circuito Meio Somador tem este nome porque não leva em consideração os resultados de somas menos significativas. Para casos em que a entrada menos significativa (denominada carry) seja considerada, usamos a denominação de circuitos de Somador Completo. Esses circuitos executam a soma dos 2 bits levando em consideração as entradas menos significativas de bit de carry. Este somador tem as mesmas saídas do Meio Somador (Soma e Carry).

![[Pasted image 20240807164421.png]]

> [!NOTE] Atenção
> Esse é o circuito somatório possível mais simples que existe.
> existem diversos outros, como o Full Adder, que tem a capacidade de armazenar um número que será adicionado a outra casa decimal,(1 + 1 = 0, vai 1), e Também o 8 bit ripple carry adder que é milhares de vezes mais complexo.
>

Um *Ripple carry* funciona da mesma maneira que a maioria dos métodos de adição com lápis e papel. Começando na posição do dígito mais à direita (menos significativo), os dois dígitos correspondentes são somados e um resultado é obtido. Um 'carry' pode ocorrer se o resultado exigir um dígito mais alto; por exemplo, **"9 + 5 = 4, carry 1".** A aritmética binária funciona da mesma maneira, com menos dígitos. Neste caso, existem apenas quatro operações possíveis, **0+0, 0+1, 1+0 e 1+1; o caso 1+1 gera um carry.** Conseqüentemente, todas as posições de dígitos, exceto a mais à direita, precisam aguardar a possibilidade de adicionar um 1 extra a partir de uma continuação dos dígitos uma posição à direita.

### Intel 74181 - Logic Unit

Intel 74181 foi uma unidade aritmética e lógica criada nos anos 70, foi a primeira ULA desenvolvida em um único chip.

provida de mais de 75 portas lógicas diferentes, era capaz de realizar todas as operações matemáticas(divisão e multiplicação eram somas e subtrações simultâneas), era capaz de decrementar, incrementar, utilizar de portas lógicas AND, NAND, OR, entre muitas outras.

1. Possui entrada para apenas 4-bits.

![[Pasted image 20240807171355.png]]

> Chip Que possui entrada e saída de 8-bits.