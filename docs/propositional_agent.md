# Agente baseado em lógica proposicional

Para criar um agente com base na lógica proposicional, a primeira etapa é permitir que o agente deduza o estado do mundo a partir de seu histórico de percepções, na medida do possível. Isso exige a criação de um modelo lógico completo das consequências das ações. Também precisamos que o agente mantenha o controle do mundo sem ter de retornar ao histórico de percepções para cada inferência. Por fim, garantimos que o agente desenvolva planos que garantam o cumprimento de seus objetivos usando inferência lógica. [9]

## Conceitos a serem considerados

- **Fluente:** Também conhecida como variável de estado, refere-se a uma variável ou aspecto do mundo que muda com o tempo. [1]
- **Variáveis atemporais:** Símbolos associados com aspectos permanentes do mundo. [1]
- **Modelo de transição:** No caso de agentes baseados em lógica proposicional, o modelo de transição (que mostra a quais estados levam certas ações) deve ser representado como um conjunto de sentenças lógicas. Este é composto por: [1]
    - **Axiomas de efeito:** Especifica o resultado futuro de uma ação específica. [1]
    - **Axiomas de quadro:** Explicitamente afirmam todas as proposições que permanecem iguais. [1]
    - **Axioma do estado sucessor:** São usados para saber como o estado de um fluente muda em resposta a uma ação. [1]
    - **Axiomas de pré-condição:** Especifica quais condições devem ser cumpridas para que uma ação específica possa ser executada com sucesso. [1]
    - **Axiomas de exclusão de ação:** Especifica que ações não podem ser executadas ao mesmo tempo. Ou seja, enquanto a ação A é executada, a ação B não pode ser executada e vice-versa. [1]
- **Localidade:** Propriedade em que as ações afetam apenas um pequeno número k de fluentes. [1]
- **Estado de crença:** Representação do conjunto de todos os possíveis estados atuais do mundo. [1]
- **Estimativa de estado:** O processo de atualização do estado da crença à medida que surgem novas percepções. [1]
- **Aproximação conservadora:** Simplificações feitas em situações complexas que asseguram exatidão ao custo de completude e precisão. [1]

# Problemas encontrados

- **Problema de quadro:** Ocorre porque, embora os axiomas de efeito registrem as mudanças que ocorrem ao realizar uma ação, estes não registram as coisas que não mudam. Pode ser resolvido incluindo axiomas de quadro. [1]
- **Problema do quadro de representação:** Problema que ocorre devido ao crescimento exponencial do número de axiomas de quadro. Em um mundo com m ações diferentes e n fluentes, o conjunto de axiomas de cuadro será de tamanho O(mn). Pode ser resolvido incluindo axiomax do estado sucessor [1]
- **Problema de quadro inferencial:** Tentativa de reduzir o tempo necessário para projetar os resultados de um plano de t etapas de O(nt) para O(kt). Onde k é o número de fluentes afetados e n é o número total de fluentes. [1]
- **Problema de qualificação:** Problema que consiste em tentar especificar todas as condições que devem ser cumpridas para que as ações sejam executadas com sucesso. [1]