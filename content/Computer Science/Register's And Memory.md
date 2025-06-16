---
tags:
  - ComputerScience
Datatime: 08/08/2024
Conteúdo: Como funcionar o gerenciamento de memoria, e o uso de registradores para isso.
---
# Register's And Memory

### And-Or Latch (Flip-Flop)

m _**flip-flop**_, **[multivibrador](https://pt.wikipedia.org/wiki/Multivibrador "Multivibrador") [biestável](https://pt.wikipedia.org/wiki/Biest%C3%A1vel "Biestável")**, ou simplesmente **biestável**, é um circuito digital que pulsado é capaz de servir como uma memória de um bit.
Um _flip-flop_ tipicamente inclui zero,um ou dois sinais de entrada, um sinal de relógio, e um sinal de saída.

O flip-flop pode ser utilizado para armazenar um [bit](https://pt.wikipedia.org/wiki/Bit "Bit"), ou um digito binário de informação. A informação armazenada em um conjunto de flip-flops pode representar o estado de um sequenciador, o valor de um contador um carácter ASCII em uma memória de um computador ou qualquer outra parte de uma informação.

![[Pasted image 20240807205544.png]]

### Registradores

é a memória dentro da própria CPU que armazena _n_ bits. Os registradores estão no topo da [hierarquia de memória](https://pt.wikipedia.org/wiki/Hierarquia_de_mem%C3%B3ria "Hierarquia de memória"), sendo assim, é um tipo de memória mais rápida e financeiramente mais custosa.
Lembrando que os registradores são circuitos digitais capazes de armazenar e deslocar informações binárias, e são tipicamente usados como um dispositivo de armazenamento temporário.

1. Registradores contemn inúmeros circuitos digitais capazes de armazenar bits, como o And-Or Latch e vários outros.  
2. Um grupo de *latches* operando é chamado de registrador
3. a quantidade de bits que um register pode aguentar é chamada de *width*.

![[Pasted image 20240807211047.png]]
> 8-Bit Register Operater.

### Memory Adress

Como você pode notar acima, se utiliza-se o formato acima mostrado, era necessário 8 cabos de dados + 8 cabos para ativar o armazenamento de memória, isso custaria horrores se fosse preciso armazenar 256 bits.

Por isso a solução encontrar é organizar os flips-flops em formato de Matrix, onde poderia ser ativado qualquer flip-flop, sem interferir em ativar outros ao seu lado.

![[Pasted image 20240807212258.png]]

![[Pasted image 20240807212324.png]]

nesse formato, caso eu deseje utilizar o segundo flip-flop, eu mandaria um sinal pela linha 1, coluna 2 para ativar esse flip-flop.
para o cabo da data eu apenas precisaria de 1 cabo que mandaria os dados a todos os flip-flops, mas como apenas 1 está ativado, nenhum outro irá fazer algo com esse dado.
a mesma coisa é feita quando eu quero informar se quero armazenar o dado ou libera-lo, eu passo essa informação a todos os flip-flop e apenas o ativado saberá realizar essa função.

#### Physical addresses

Na computação, um endereço de memória é uma referência a um local específico de memória usado em vários níveis por software e hardware. Endereços de memória são sequências de dígitos de comprimento fixo convencionalmente exibidos e manipulados como números inteiros sem sinal.

Cada local de memória possui um endereço físico que é um código. A CPU (ou outro dispositivo) pode usar o código para acessar o local de memória correspondente. Geralmente apenas software de sistema ou a BIOS.

O barramento dos controladores de memória consiste em várias linhas paralelas, cada uma representada por um dígito binário (bit). A largura do barramento e, portanto, o número de unidades de armazenamento endereçáveis ​​e o número de bits em cada unidade variam entre os computadores.

### Multiplexer

é um dispositivo que seleciona as informações de duas ou mais fontes de dados num único canal. São utilizados em situações onde o custo de implementação de canais separados para cada fonte de dados é maior que o custo e a inconveniência de utilizar as funções de multiplexação/demultiplexação.

A função básica de um multiplexador é combinar múltiplas entradas num único terminal de dados. No lado da recepção um [demultiplexador](https://pt.wikipedia.org/wiki/Demultiplexador "Demultiplexador") divide o fluxo único de dados nos sinais múltiplos originais.

1. quando deseja se utilizar um flip-flop especifico, passamos seu endereço em binário que representa a sua posição na linha/coluna,*(exemplo: 0001 = 1 linha)*, o multiplexer irá fazer essa conversão muito mais rápido tanto para a coluna, tanto para a linha.     

![[Pasted image 20240807215553.png]]

Para conseguir salvar um pequeno número como um byte, precisa-se de 8 256-bit memory, onde cada bit será salvo no mesmo local nos 8 locais de memória.

Dessa forma, esse registrador é capaz de armazenar 256 bytes em 256 locais diferentes.

![[Pasted image 20240807215933.png]]

Tudo, Exatamente Tudo que já foi dito até agora foi apenas para caracterizar um componente que existe em qualquer computador da história humana, Memória.

Atualmente Conhecida como **RAM**(Random Access Memory), que tem como função guardar aleatoriamente memory pelo tempo que o computador está realizando uma função.