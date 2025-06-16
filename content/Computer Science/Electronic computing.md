---
tags:
  - ComputerScience
Datatime: 05/08/2024
Conteúdo: Computadores eletrônicos, componentes e evolução.
---
# Computadores Digitais

Após anos de desenvolvimento e criação de diversos computadores, em 1938, os computadores totalmente elétricos substituíram os computadores eletromecânicos.

Estes foram os primeiros computadores digitais que funcionavam a base de [tubos de vácuo](https://pt.wikipedia.org/wiki/V%C3%A1lvula_termi%C3%B4nica "Válvula termiônica").

### Konrad Zure

Em 1941, Zuse seguiu sua máquina anterior com o [Z3](https://pt.wikipedia.org/wiki/Z3 "Z3"), o primeiro computador digital eletromecânico [programável](https://pt.wikipedia.org/wiki/Programa%C3%A7%C3%A3o_de_computadores "Programação de computadores") e totalmente automático do mundo.

O Z3 foi construído com 2.000 [relés](https://pt.wikipedia.org/wiki/Rel%C3%A9 "Relé"), implementando um [comprimento de palavra](https://pt.wikipedia.org/wiki/Palavra_(ci%C3%AAncia_da_computa%C3%A7%C3%A3o) "Palavra (ciência da computação)") de 22 [bits](https://pt.wikipedia.org/wiki/Bit "Bit") que operava em uma [frequência de clock](https://pt.wikipedia.org/wiki/Frequ%C3%AAncia_de_clock "Frequência de clock") de cerca de 5–10 [Hz](https://pt.wikipedia.org/wiki/Hertz "Hertz").

O código do programa foi fornecido em filme perfurado enquanto os dados podiam ser armazenados em 64 palavras de memória ou fornecidos pelo teclado. Era bastante semelhante às máquinas modernas em alguns aspectos, sendo pioneiro em vários avanços, como os números de pontos flutuantes.

Em vez do sistema decimal mais difícil de implementar (usado no projeto anterior de [Charles Babbage](https://pt.wikipedia.org/wiki/Charles_Babbage "Charles Babbage")), o uso de um sistema [binário](https://pt.wikipedia.org/wiki/Sistema_de_numera%C3%A7%C3%A3o_bin%C3%A1rio "Sistema de numeração binário") significava que as máquinas de Zuse eram mais fáceis de construir e potencialmente mais confiáveis, dadas as tecnologias disponíveis na época.

### Tubos de vácuo e circuitos eletrônicos digitais

Os elementos de [circuitos puramente eletrônicos](https://pt.wikipedia.org/wiki/Circuito_eletr%C3%B4nico "Circuito eletrônico") logo substituíram seus equivalentes mecânicos e eletromecânicos, ao mesmo tempo em que o cálculo digital substituiu o analógico.

Os **circuitos eletrônicos** diferem dos circuitos elétricos por possuírem interligações entre diversos componentes eletrônicos, enquanto os circuitos elétricos somente têm conexões entre componentes elétricos.


### Havard Mark 1

chamado popularmente de **Mark I**, foi a primeira [calculadora](https://pt.wikipedia.org/wiki/Calculadora "Calculadora") [eletromecânica](https://pt.wikipedia.org/wiki/Digital "Digital") automática produzida em larga escala.

O ASCC foi construído a partir de [interruptores](https://pt.wikipedia.org/wiki/Interruptor "Interruptor"), [relés](https://pt.wikipedia.org/wiki/Rel%C3%A9 "Relé"), [eixos rotativos](https://pt.wikipedia.org/wiki/Eixo_(mec%C3%A2nica) "Eixo (mecânica)") e [embreagens](https://pt.wikipedia.org/wiki/Embraiagem "Embraiagem"). Utilizou 765 mil componentes [eletromecânicos](https://pt.wikipedia.org/wiki/Eletromec%C3%A2nica "Eletromecânica") e centenas de [quilômetros](https://pt.wikipedia.org/wiki/Quil%C3%B4metro "Quilômetro") de fio.

1. Mechanical Relay. era um tipo de passagem de energia que utilizava um cano condutor de energia, onde esse cano era conectado a sua outra parte se um sinal (Control Wire) fosse enviado.
2. Caso o sinal fosse enviado, energia suficiente era passado para um mecanismo abaixo do cano, que ficaria magnetizado e conectaria o cano acima. (Como o fechar e abrir de uma torneira, so que com magnetismo.)

3. ![[Pasted image 20240805132631.png]]

O problema desse mecanismo era o delay absurdo criado, já que as conexões criadas era feitas por ações físicas,
e não digitais.

além do problemas de troca-las, já que o computador Mark 1 possui-a 3500 relays, aonde cada uma tinha uma vida útil de 10 anos. +- uma troca por dia.


### O primeiro Bug de computador.

Em uma noite de 9 de setembro de 1947,Enquanto trabalhavam no computador, a equipe de Hopper enfrentou um problema inexplicável: o computador simplesmente parou de funcionar. Após uma investigação minuciosa, eles descobriram a causa do mau funcionamento: uma mariposa havia ficado presa no Relé #70, Painel F, interrompendo o fluxo elétrico, causando um curto-circuito e o "bug" no sistema. Os operadores removeram e afixaram a mariposa no registro do computador, com a entrada: "First actual case of bug being found"  (Primeiro caso real de bug encontrado). Eles divulgaram que haviam “depurado” a máquina, introduzindo assim o termo “depurando um programa de computador”.

Ela adotou o termo "bug" para descrever falhas de programação, uma terminologia que ainda é usada hoje. Desde então, o termo "bug" se tornou parte integrante da linguagem da computação, utilizado para descrever qualquer problema ou falha em um sistema computacional, até mesmo em coisas do dia a dia.

### ENIAC

(Electronic Numerical Integrator and Computer) foi o primeiro computador eletrônico programável construído nos Estados Unidos. Embora fosse semelhante ao Colossus, era muito mais rápido, mais flexível e tinha [Turing completude](https://pt.wikipedia.org/wiki/Turing_completude "Turing completude"). Assim como o Colossus, um “programa” no ENIAC era definido pelos estados de sues patch cables e switches, muito longe dos programas armazenados nas máquinas eletrônicas que vieram depois. Depois que um programa era escrito, ele precisava ser configurado mecanicamente na máquina com reinicialização manual de plugues e interruptores.

Ele combinava a alta velocidade da eletrônica com a capacidade de ser programado para muitos problemas complexos. Podia somar ou subtrair 5 mil vezes por segundo, mil vezes mais rápido do que qualquer outra máquina. Também tinha módulos para multiplicar, dividir e raiz quadrada.

A máquina era enorme, pesando 30 toneladas, consumindo 200 quilowatts de energia elétrica e continha mais de 18 mil tubos de vácuo, 1.500 relés e centenas de milhares de resistores, capacitores e indutores.

- [ ] Menção honrosa ao Colossus, computador anterior ao ENIAC que foi importantíssimo para a criação do próprio ENIAC. 