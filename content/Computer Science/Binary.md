---
tags:
  - ComputerScience
Datatime: 05/08/2024
Conteúdo: Sistema de base 2, altamente utilizado na programação e computadores.
Linked:
  - "[[Boolean,Gates Logic]]"
  - "[[Electronic computing]]"
---
# Binary

O sistema binário ou de base 2 é um sistema de numeração posicional em que todas as quantidades se representam com base em dois números,ou seja, zero e um.

Os computadores digitais trabalham internamente com dois níveis de tensão, pelo que o seu sistema de numeração natural é o sistema binário.Com efeito, num sistema simples como este é possível simplificar o cálculo, com o auxílio da lógica booleana.

1. cada dígito binário é representado por um bit,(0 ou 1).
2. Um agrupamento de 8 bits é chamado de byte.

Um processador é formado por milhares de blocos lógicos complexos, formados por portas lógicas básicas, e o funcionamento destas está amparado por um postulado fundamental à eletrônica digital que determina que um circuito opere apenas com dois níveis de tensão bem definidos.

Em um [circuito digital](https://pt.wikipedia.org/wiki/Circuito_digital "Circuito digital") [TTL](https://pt.wikipedia.org/wiki/L%C3%B3gica_transistor-transistor "Lógica transistor-transistor"), dois níveis de tensão padronizados são 0V e 5V. Ao projetar um sistema digital, ao invés de trabalhar com níveis de tensão trabalha-se com níveis lógicos, então, no caso do circuito TTL, 0V será representado por “0” e 5V será representado por “1”, e os níveis de tensão entre eles serão ignorados, ou seja, adotar-se-á uma faixa até a qual será considerado nível lógico zero, e a partir dela, nível lógico 1. Neste caso, de 0V a 2,5V temos “0”, e a partir daí até 5V temos “1”.


*O sistema binário é base para a Álgebra booleana, que permite fazer operações lógicas e aritméticas usando-se apenas dois dígitos ou dois estados (sim ou não, verdadeiro ou falso, tudo ou nada, ligado ou desligado, 1 ou 0).*

### Importância

Toda a electronica digital e computação estão baseadas nesse sistema binário e na lógica de boole,que permite representar por circuitos electrónicos digitais (portas lógicas) os números, caracteres, realizar operações lógicas e aritméticas. Os programas de computadores são codificados sob forma binária e armazenados nas mídias (memórias, discos, etc) sob esse formato.

Assim, para informação armazenada na memória RAM do computador, o formato será de voltagem mais alta (1) ou mais baixa (0).

### Bits na computação

8 bits é uma referência aos processadores antigos que apenas utilizavam 8 bits para executar suas ações.

além dos processadores, esse formato foi amplamente usado na década de 70 principalmente em videos e imagens.

1. Em um video, o formato 8 bits podia apenas representar 256 valores diferentes, ou seja, apenas 256 cores podiam ser mostradas por frame/execução do video.
2. já o formato 24 bits, que foi desenvolvidos anos depois, podia suportar até 16,777,216 cores por ação.

### 32-BIT / 64-BIT
**32 bits** e **64 bits** são especificações ligadas à arquitetura de um sistema e se referem à quantidade de dados que um chip pode processar por vez.
O número de bits determina o tamanho máximo do dado que pode ser processado durante uma operação.

Durante um cálculo, os valores envolvidos são transferidos da memória do computador para os registradores. Se os registradores suportam 64 bits, eles permitirão que a CPU faça cálculos maiores ou mais rapidamente do que se eles contassem com 32 bits ou menos.

![[Pasted image 20240805204845.png]]

### Números Negativos.

Em representações reais, números positivos e negativos são diferenciados por um prefixo, ( + , -).

No entanto,em um Hardware computacional, os números são representados em binário apenas, sem símbolos extras, requerendo um método de codificação para números negativos.

Atualmente existem 4 métodos para entender o sistema binário:

**Complemento para um**,
**Complemento para dois**,
**Sinal-e-Magnitude** e
**Excesso-N**.

A representação de **sinal-e-magnitude** ou **sinal-magnitude** é a mais familiar a nós que utilizamos o sistema numérico de base 10, usando um sinal positivo ou negativo à esquerda do número para indicar se este é positivo ou negativo.

*00000000 = +0 ou 0*
*00000001 = 1 ou 1*
*10000000 = -0 ou 128*
*10000001 = -1 ou 128*

**complemento para um** ou **complemento de um** pode ser usado para representar números negativos. A forma de representar números negativos em "complemento para um" é aplicar a operação [bitwise NOT](https://pt.wikipedia.org/wiki/Porta_NOT "Porta NOT") para os números negativos (com -), ou seja, o complemento da sua contraparte positiva.

*00101011 = 43 // 11010100 = -43*
Inverte o número e obtém seu negativo.

Os problemas de múltiplas representações de 0 e a necessidade de tratamento com "vai-um" são contornadas por um sistema chamado **complemento para dois**.Em **complemento para dois**, há apenas um zero (00000000). Se nega um número (negativo ou positivo) invertendo-se todos os bits e, em seguida, adicionando 1 ao resultado.

*00000000 = -127 ou 0*
*0000001 = -126 ou 1*
cada bit adicionado ao número, diminui a casa negativa, aumenta a casa positiva.

### Float Numbers - Binário.
números floats são números que representam casas decimais, por exemplo 3,14.

Os números de ponto flutuante usam o formato *IEEE*.Os valores de precisão simples com tipo float têm 4 bytes, que consistem em um bit de sinal, um expoente binário de 8 bits no formato de 127 em excesso e uma mantissa de 23 bits. A mantissa representa um número entre 1,0 e 2,0. Como o bit de ordem superior da mantissa é sempre 1, ele não é armazenado no número. Essa representação fornece um intervalo de aproximadamente 3,4E-38 a 3,4E+38 para o tipo float.

![[Pasted image 20240805212055.png]]

Assim o número 625.9 pode ser representado por:

0.6259 x 10³

onde 0.6259 é considerado o significativo,
e o 10³ o expoente.

### Tabela ASCII

é um sistema de representação de letras, algarismos e sinais de pontuação e de controle, já que se via necessário criar um modelo baseado em binário que não apenas representassem os números, mas letras e outros diversos textos.

desenvolvido em 1960, representa um conjunto de 128 sinais: 95 sinais gráficos e 33 sinais de controle ,utilizando 7 bits para representar todos os seus símbolos.

> [!NOTE] Atenção
> Talvez você tenha notado que a tabela ASCII tem tamanho 1 byte, mas apenas usa 7 bits, porque?. porque esse bit excedente pode ser utilizado de varias formas que apenas depende de como for aplicado. por exemplo, o padrão UTF-8 o utiliza para identificar que o valor excedeu o número limite 128. 

A codificação ASCII é usada para representar textos em computadores, equipamentos de comunicação, entre outros dispositivos que trabalham com texto. Desenvolvida a partir de grande parte das codificações de caracteres modernas a herdaram como base.

Os sinais não-imprimíveis, conhecidos como caracteres de controle, são amplamente utilizados em dispositivos de comunicação e afetam o processamento do texto.

- [ ] Também existe uma versão Extend da Tabela ASCII, que usa esse bit extra para adicionar caracteres que podem representar funções, números específicos entre diversos outros. 

### Unicode
porém existia um grande problema com o padrão UTF-8, como diabos caberia em um único complemento de 8 bits, diversos caracteres de diversas linguagens existentes no mundo?, como a japonesa, a russa, a chinesa, e todas as outras.

1. esse problema deixou diversas transferências de textos entre línguas completamente ilegíveis, ocasionando na criação de um próprio padrão por cada país.   

**É aqui que entra o UNICODE**

**Unicode** é um padrão permite aos computadores representar e manipular, de forma consistente, texto de qualquer sistema de escrita existente.

o padrão consiste de quase 138 mil caracteres um conjunto de diagramas de códigos para referência visual, uma metodologia para codificação e um conjunto de codificações padrões de caracteres, uma enumeração de propriedades de caracteres como Uppercase e Lowercase, um conjunto de arquivos de computador com dados de referência, além de regras para normalização, decomposição, ordenação alfabética e renderização.

Seu sucesso em unificar conjuntos de caracteres levou a um uso amplo e predominante na internacionalização e localização de programas de computador. O padrão foi implementado em várias tecnologias recentes, incluindo [XML](https://pt.wikipedia.org/wiki/XML "XML"), [Java](https://pt.wikipedia.org/wiki/Plataforma_Java "Plataforma Java") e sistemas operacionais modernos.