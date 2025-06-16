---
tags:
  - ComputerScience
Datatime: ""
Conteúdo: Funcionamento e Design de CPU avançadas.
Linked:
  - "[[Arithmetic & Logic Unit]]"
  - "[[CPU - Unidade Central de Processamento.]]"
  - "[[Register's And Memory]]"
Reference:
---
# Advance CPU Design

Ao longo dos anos, computadores super rápidos foram desenvolvidos. todos esses computadores foram se tornando mais rápidos por causa que os transistores foram se tornando cada vez mais tecnológicos. 

Todos esses anos, foram em base em um único design, para deixar os computadores mais rápidos, vamos deixa-los mais complexos.

Hoje em dia, computadores possuem diversas instruções imediatas para compressão de video, cryptographer arquivos, operações avançadas e diversos outros. 

Só que mesmos com esses avanços, existe um pequeno problema.
**transferência de dados**.

### Bus Cable --Barramento

Na computação, um barramento é conhecido como um sistema de comunicação que transfere dados entre componentes. Um exemplo seria um USB. USB significa Universal Serial Bus e muitos dispositivos usam este cabo, conector e protocolo para interagir com um computador.
Os primeiros barramentos de computador eram fios elétricos paralelos com múltiplas conexões de hardware, mas o termo agora é usado para qualquer arranjo físico que forneça a mesma função lógica de um [barramento elétrico](https://pt.wikipedia.org/wiki/Barramento "Barramento") paralelo.

### Memory Cache
Por causa da diferença entre os desempenhos da CPU e da Memoria, um novo tipo de memoria foi criado para operar e transferir dados em velocidades parecidas com a da CPU, a **memoria Cache**.

 Ela tem o objetivo de reduzir o tempo médio de acesso aos dados armazenados na memória. A cache é uma memória de pouco espaço, porém muito mais rápida e armazena as informações que são usadas com mais frequência pela CPU.

esses sistemas, as CPUs se comunicam usando barramentos de alto desempenho que operam em velocidades muito maiores que a memória, e se comunicam com a memória usando protocolos semelhantes aos usados ​​exclusivamente para periféricos no passado.

#### Funcionamento

1. Quando a CPU necessita de um determinado endereço que está armazenado na memória, o primeiro lugar a buscar este endereço é na memória cache. Se o conteúdo está na cache, ocorre o acerto na cache, chamado de _cache hit_ (quando o conteúdo requisitado pelo CPU é encontrado na cache), fazendo a informação ser acessada pela CPU sem necessidade de acesso à memória principal. Se o conteúdo não está na cache, ocorre uma falta de cache, chamado de _cache miss_ (quando o conteúdo requisitado pela CPU não esta presente na cache), o que leva a CPU a buscar essa informação na memória principal. Como provavelmente essa informação será requisitada novamente (localidade temporal) o dado que foi buscado na RAM é copiado na cache.
2. Como a cache possui capacidade de armazenamento extremamente limitada (algo comum de acontecer devido ao seu custo), os novos dados que chegam da memória principal precisam ocupar o lugar de dados já presentes na cache provocando assim a evasão de dados menos recentes.

### Dirty bit
bit sujo ou bit modificado, é um bit que é associado com um bloco de memoria que foi modificado. esse bit é setado quando o processador altera dados por exemplo na cache, mais não salva esses mesmos dados na memoria.
Esse efeito causa uma diferença entre os valores da *memoria cache e memoria RAM*.Mas, esse Dirty bit é responsável por resolver esse efeito.
Para isso, esse bit, no momento em que esse bloco de memoria vai ser trocado, ele check se o bloco de memoria precisa ser salvo na memoria Ram, caso não precise ser salvo, ele apenas será trocado por outro bloco de memoria.

Bits sujos são usados ​​pelo cache da CPU e nos algoritmos de substituição de página de um sistema operacional.


