# Agente baseado em conhecimento

Os agentes baseados em conhecimento são aqueles que têm a capacidade de manter um estado interno de conhecimento, raciocinar sobre esse conhecimento, atualizar seu conhecimento após observações e realizar ações. Esses agentes podem representar o mundo com alguma representação formal e agir de forma inteligente. [2]

Um agente baseado no conhecimento deve ser capaz de realizar as seguintes ações:

- Um agente deve ser capaz de representar estados, ações, etc. [2]
- Um agente deve ser capaz de incorporar novas percepções. [2]
- Um agente pode atualizar a representação interna do mundo. [2]
- Um agente pode deduzir a representação interna do mundo. [2]
- Um agente pode deduzir ações apropriadas. [2]

## Base de conhecimento

O componente central desse agente é a base de conhecimento, que é composta por frases, que é uma afirmação do mundo real representada usando linguagem de representação do conhecimento. Uma frase que não é derivada de outras frases é conhecida como axioma. Para obter novas frases, usa-se um processo chamado inferência, no qual frases já estabelecidas são usadas para gerar novas frases. A base de conhecimento também contém um conjunto de frases iniciais, estes são chamados de conhecimentos prévios. [1]

## Sistema de inferência

Ele é usado quando você quer atualizar informações em um sistema baseado no conhecimento e também para conhecer a informação que já tem. Este mecanismo é realizado através das operações TELL e ASK. [3]

**Ações realizadas:**

1. Ele DIZ (TELLS) o que reconheceu do ambiente e o que precisa saber para a base de conhecimento. [3]
2. Ele PERGUNTA (ASKS) quais ações fazer e obtém respostas da base de conhecimento. [3]
3. Ele DIZ (TELLS) à base de conhecimento qual ação foi selecionada e, em seguida, o agente executa essa ação. [3]

## Exemplo de agente baseado em conhecimento

```

function KB-AGENT(percept):  
persistent: KB, a knowledge base   
          t, a counter, initially 0, indicating time   
TELL(KB, MAKE-PERCEPT-SENTENCE(percept, t))   
Action = ASK(KB, MAKE-ACTION-QUERY(t))   
TELL(KB, MAKE-ACTION-SENTENCE(action, t))  
 t = t + 1  
 return action

```

O **MAKE-PERCEPT-SENTENCE** gera uma frase que define que o agente percebeu a percepção em questão em um determinado momento. [2]

O **MAKE-ACTION-QUERY** gera uma sentença para perguntar qual ação deve ser executada no momento atual. [2]

O **MAKE-ACTION-SENTENCE** gera uma frase que afirma que a ação escolhida foi executada. [2]

## Níveis de agentes baseados em conhecimento

### Nível de conhecimento

O nível de conhecimento é o primeiro nível do agente baseado em conhecimento e, nesse nível, precisamos especificar o que o agente sabe e quais são os objetivos do agente. Com essas especificações, podemos fixar seu comportamento. Por exemplo, suponha que um agente de táxi automatizado precise ir de uma estação A para a estação B e que ele saiba o caminho de A para B, portanto, isso está no nível de conhecimento. [2]

### Nível lógico:

Nesse nível, entendemos como a representação do conhecimento é armazenada. Nesse nível, as sentenças são codificadas em diferentes lógicas. No nível lógico, ocorre uma codificação do conhecimento em sentenças lógicas. No nível lógico, podemos esperar que o agente de táxi automatizado chegue ao destino B. [2]

### Nível de implementação:

Essa é a representação física da lógica e do conhecimento. No nível de implementação, o agente executa ações de acordo com o nível lógico e de conhecimento. Nesse nível, um agente de táxi automatizado realmente implementa seu conhecimento e lógica para que possa chegar ao destino. [2]

## Abordagens de agentes baseados em conhecimento

**Abordagem declarativa:** Nesse caso, partindo de uma base de conhecimento vazia, o agente pode DIZER frases uma após a outra até que tenha conhecimento de como trabalhar com seu ambiente. Isso é conhecido como abordagem declarativa. Ela armazena as informações necessárias em um sistema vazio baseado em conhecimento. [3]

**Abordagem processual:** Converte os comportamentos necessários diretamente em código de programa em um sistema vazio baseado em conhecimento. É uma abordagem de contraste quando comparada à abordagem declarativa. Nela, o comportamento de codificação do sistema é projetado. [3]