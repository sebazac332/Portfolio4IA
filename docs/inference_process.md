# Processo de inferência

Aqui olhamos como a vinculação pode ser feita por meio da comprovação de teoremas, aplicando regras de inferência diretamente às sentenças em nossa base de conhecimento para construir uma prova da sentença desejada sem consultar modelos. Se o número de modelos for grande, mas o comprimento da prova for pequeno, a prova de teoremas pode ser mais eficiente do que a verificação de modelos.  [1]

**Conceitos de fundo:**

- **Equivalência lógica:** Duas frases A e B são logicamente equivalentes se forem verdadeiras nos mesmos modelos. Em outras palavras, quaisquer duas sentenças a e b são equivalentes se e somente se cada uma delas implicar a outra. [1]

- **Validade:** Uma frase é válida se for verdadeira em todos os modelos. Essas frases também são conhecidas como tautologias, elas são necessariamente verdadeiras. [1]

- **Satisfatoriedade:** Uma frase é satisfatória se for verdadeira em algum modelo ou for satisfeita por ele. A satisfatoriedade pode ser verificada enumerando os modelos possíveis até encontrar um que satisfaça a frase. [1]

## Inferência e provas

Esta seção aborda as regras de inferência que podem ser aplicadas para derivar uma prova

- **Modus Ponens:** Se uma declaração condicional (declaração “if-then”) for verdadeira e seu antecedente (a parte “if”) for verdadeiro, então seu consequente (a parte “then”) também deverá ser verdadeiro. [4]

- **And-Elimination:** Regra que diz que, a partir de uma conjunção, qualquer um dos conjuntos pode ser deduzido. [1] Em outras palavras, se uma conjunção (uma declaração “and”) for verdadeira, então cada um de seus conjuntos também será verdadeiro. [4]

- **Eliminação bicondicional:** A eliminação bicondicional nos permite deduzir uma implicação e seu inverso de uma bicondicional. [5] Em outras palavras, se você sabe que P <=> Q, pode concluir P => Q. Da mesma forma, pode concluir Q => P. [6]

- **Equivalência lógica para contrapositivos:**  A afirmação condicional e sua contrapositiva são logicamente equivalentes: p => q <=> ∼q => ∼p. Em outras palavras, a afirmação original e a contrapositiva devem concordar uma com a outra. Ambas devem ser verdadeiras, ou ambas devem ser falsas. [7]

- **Regra de De Morgan:** A lei de De Morgan é a lei que fornece a relação entre E, OU ou negação da declaração. Representando a regra de De Morgan este é assim ∼ (a ∧ b) ≡ ∼ a ∨ ∼ b e ∼ (a ∨ b) ≡ ∼ a ∧ ∼ b. [8]