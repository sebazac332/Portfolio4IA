# Lógica

Nesta parte veremos os conceitos fundamentais da representação lógica e do racionciio, que se aplicam independentemente de qualquer forma lógica em particular. [1]

**Syntax:** É a estrutura que segue a linguagem de representação lógica quando se trata de representar uma frase. Por exemplo, na aritmética, a sintaxe define que uma representação correta de uma frase é x + y = 4 enquanto que uma representação incorreta seria x4y +=. [1]

**Semanticas:** Também conhecido como o significado de uma frase, é uma verdade de cada frase em relação a um mundo específico possível. Por exemplo, a frase acima apresentada x + y = 4 é verdadeira em um mundo possível onde x é 2 e y é 2, mas essa mesma frase é falsa em um mundo possível onde x é 1 e y é 1. [1]

**Modelo:** São abstrações matemáticas de ambientes reais potenciais em que o agente pode ser encontrado (mundos possíveis). Eles atribuem valores às variáveis relevantes e têm um valor fixo (verdadeiro e falso) para cada frase especificada. Por exemplo, na frase anterior x + y = 4 os modelos possíveis são atribuições de valores inteiros não negativos para as variáveis x e y. [1]

**Satisfação:** Ocorre quando uma frase "a" é verdadeira quando está em um modelo "M". Quando isso acontece, pode-se dizer que "M" satisfaz a a ou que "M" é um modelo de "a". O conjunto de modelos que satisfazem a frase "a" é representado usando a notação M(a). [1]

**Implicação:** É a ideia de que uma frase segue logicamente de outra frase. Isto é, assumindo que se tem duas frases a e b, em qualquer modelo em que a é verdade b também será verdade. Um exemplo de uma ligação séria que a frase x = 0 verdadeira implica que a frase xy = 0 também é verdadeira. A notação |= é usada para representar uma implicação, cuando A implica B se representa A |= B. [1]

## Propriedades de algoritmos

Aqui são apresentadas propriedades de algoritmos baseados em conhecimento que são muito desejadas.

**Preservação da verdade:** Também conhecido como solidez, é quando todas as conclusões derivadas são devido a que seguem logicamente da base de conhecimento. Um processo de inferência que não é sólido basicamente inventa coisas durante a execução. [1]

**Completude:** É quando um algoritmo é capaz de derivar todas as frases que seguem logicamente a base de conhecimento. Quando se aplica algoritmos a espaços infinitos esta propriedade representa um problema bastante grande. [1]

**Aterramento:** É a conexão entre os processos de raciocínio lógico e o ambiente real em que o agente existe. Como se sabe que a base de conhecimento é verdadeira no mundo real? A resposta mais simples é que os sensores do agente fazem essa conexão. [1]