---
tags:
  - ComputerScience
Datatime: 12/08/2024
Conteúdo: Componente principal de um computador.
Linked:
  - "[[Arithmetic & Logic Unit]]"
  - "[[Register's And Memory]]"
  - "[[Advance CPU Design]]"
  - "[[Binary]]"
---
# Central Processing Unit
Todos os programas de computadores, softwares, jogos e aplicativos, são feitos de series de operações individuais, chamadas de instruções.

1. Se essas instruções forem pequenas operações matemáticas, a CPU envia essas operações para serem executadas na [[Arithmetic & Logic Unit]] (ULA).

2. Ou essas instruções são instruções de memoria, aonde o CPU enviará esses dados para serem lidos e armazenados pela memoria [[Register's And Memory]] (RAM).


### Instruction Table

Tabela de instruções ou Instruction Table, são tabelas que guardam o código em binário de diversas Instruções que o CPU pode fazer.

1. *Ex: Read Ram location into register A --4-BIT-CODE 0010*

![[Pasted image 20240812190927.png]]

## Fases de uma CPU

#### Fetch Phase
Fetch Phase, é a fase da CPU aonde o [Instruction Address Register] é responsável por receber os valores que estão localizadas na memoria, um local por vez, um código de 8-Bits por vez. e enviar esse código para o [Instruction Register].

#### Decode Phase
Nessa fase da CPU, o código que está localizado no [Instruction Register], é analisado, é verificado nessa fase, os 4 primeiros dígitos para identificar qual instrução deverá ser executada. 
**-Opcode é o nome da parte do binário que executada determinada instrução.** 

#### Execute Phase
Nessa fase, depois da instrução ser determinada pelo **Opcode**, os determinados circuitos lógicos que são responsáveis por essa instrução serão chamadas e realizaram a instrução.
 ![[Pasted image 20240812192306.png]]

Depois da instrução ser realizada, o Register Adress é incrementado em +1, para que agora seja realizado a instrução que está localizado no primeiro Adress!.

![[Pasted image 20240812192533.png]]

Existem Diversos tipos de instruções que podem ser realizados por uma CPU, diversas delas implementar lógica aritmética, como somar, diminuir, dividir e multiplicar.Para essas instruções, o [[Arithmetic & Logic Unit]] (ALU) deverá está disponível para realiza-las.

![[Pasted image 20240812193153.png]]

### Clock
O clock é um componente que realiza a função de mandar sinais elétricos para a precisão e regulação dos intervalos tornando as execuções das instruções mais organizadas e em ordens.

#### Clock Speed
é a medida de velocidade com que uma CPU consegue realizar as fase Fetch, Decode, e Execute. Essa medida é mensurável em **Hertz**.
- Uma unidade de frequência que mede a quantidade de ações realizadas por segundo. (Hertz's/Segundos).


> Brincando Um pouco agora utilizando as instruções Abaixo.

![[Pasted image 20240812195204.png]]

