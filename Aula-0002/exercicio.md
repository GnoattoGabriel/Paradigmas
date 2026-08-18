# Questões 4, 5, 10 e 11 — Conceitos de Linguagens de Programação

## 4 - Fortran: desempenho, custo e adoção

O projeto Fortran precisou convencer os programadores de que a abstração proporcionada por uma linguagem de alto nível não significaria necessariamente perda significativa de desempenho.

A estratégia foi demonstrar que o compilador poderia gerar código próximo da qualidade do código escrito à mão, enquanto a linguagem reduzia muito o esforço, o tempo e o custo de desenvolvimento.

---

## 5 - Fortran e Lisp

### Domínios diferentes

O **Fortran** foi desenvolvido para atender principalmente cientistas e engenheiros que precisavam realizar cálculos numéricos. Por isso, a linguagem foi projetada para expressar fórmulas matemáticas de maneira relativamente direta e produzir código eficiente.

O **Lisp**, por outro lado, surgiu a partir das pesquisas de **John McCarthy** em inteligência artificial. Seu objetivo estava relacionado ao processamento de informações simbólicas, uma necessidade diferente daquela encontrada na computação científica. Em vez de trabalhar principalmente com números, Lisp precisava manipular conceitos, expressões e estruturas simbólicas.

### Representação de dados

No **Fortran**, números são fundamentais. A linguagem oferece tipos e operações apropriados para cálculos científicos, além de estruturas como **arrays**, importantes para representar vetores e matrizes.

No **Lisp**, a **lista** é uma estrutura fundamental. Uma expressão Lisp pode ser representada como uma lista e, ao mesmo tempo, programas Lisp também podem ser tratados como estruturas de dados. Essa característica foi especialmente importante para a inteligência artificial, porque permitia construir, analisar e modificar estruturas simbólicas de maneira bastante flexível.

### Estilo de computação

O **Fortran** favorece um estilo voltado para cálculos e transformação de valores numéricos. O programador descreve operações matemáticas e algoritmos que serão executados sobre números, normalmente seguindo uma sequência de instruções.

O **Lisp** favorece a computação simbólica, com forte utilização de funções, listas e recursão. Em vez de simplesmente calcular números, um programa pode manipular uma expressão como uma estrutura, examinando seus componentes e construindo novas estruturas.

---

## 10 - Ortogonalidade, regularidade e simplicidade

Uma linguagem é **ortogonal** quando há poucas restrições sobre como seus recursos podem ser combinados. Por exemplo, se um determinado tipo de dado pode ser usado em uma construção, seria desejável que também pudesse ser usado em outras construções de maneira consistente.

Isso aumenta a regularidade da linguagem e facilita prever o comportamento de programas.

O **ALGOL 68** é um exemplo importante porque buscou um alto grau de ortogonalidade e regularidade. Seus projetistas procuraram construir uma linguagem na qual conceitos pudessem ser combinados de maneira sistemática, evitando muitas exceções e casos particulares.

Por exemplo, o ALGOL 68 tinha um sistema de tipos bastante geral, permitindo que diferentes tipos de dados fossem utilizados em várias construções da linguagem. Essa abordagem produzia uma linguagem regular, pois seus recursos obedeciam a princípios relativamente uniformes.

Porém, essa mesma generalidade tornou o ALGOL 68 complexo. O usuário precisava compreender muitas regras e possibilidades de combinação.

Assim, uma linguagem pode ser **regular**, isto é, consistente e com poucas exceções, sem ser necessariamente **simples** de aprender ou utilizar.

### Regularidade

Os recursos da linguagem seguem regras uniformes e previsíveis.

### Simplicidade

Existem poucos conceitos e regras que o programador precisa aprender.

### Uma linguagem muito ortogonal é automaticamente fácil de usar?

**Não.**

A ortogonalidade tende a facilitar o aprendizado porque reduz exceções e torna o comportamento da linguagem mais previsível. Porém, uma ortogonalidade excessiva pode aumentar a complexidade quando permite muitas combinações possíveis entre os recursos.

Portanto, existe uma relação de equilíbrio.

Uma linguagem com **baixa ortogonalidade** pode ser difícil porque possui muitas exceções e regras especiais.

Uma linguagem **extremamente ortogonal**, por outro lado, pode ser difícil porque oferece um grande número de combinações e conceitos gerais que o programador precisa compreender.

---

## 11 - Cadeia de influência: ALGOL, Pascal e C

### ALGOL 60 → Pascal → C

O **ALGOL 60** foi uma das principais referências para o desenvolvimento das linguagens imperativas estruturadas. Introduziu uma organização mais sistemática para estruturas de controle e influenciou fortemente linguagens posteriores.

**Pascal**, criada por **Niklaus Wirth**, recebeu forte influência do ALGOL. Seu objetivo incluía oferecer uma linguagem estruturada, relativamente simples e adequada ao ensino de programação. Pascal manteve a orientação **imperativa**, baseada em comandos que alteram o estado do programa.

**C** também pertence a essa linhagem. Foi influenciada por linguagens anteriores da família ALGOL, especialmente por sua estrutura sintática e pelo conceito de programação estruturada, embora tenha incorporado características próprias, como maior proximidade com o hardware e operações sobre memória.

### Contraste com Prolog

O **Prolog** segue uma proposta bastante diferente. Enquanto ALGOL, Pascal e C pertencem predominantemente ao paradigma **imperativo**, Prolog é uma linguagem **lógica/declarativa**.

Nas linguagens imperativas, o programador descreve **como** o computador deve realizar uma tarefa. Um programa é composto por comandos, atribuições, estruturas de repetição e decisões que determinam uma sequência de ações e modificam o estado da memória.

Em **Prolog**, o programador descreve principalmente **o que é verdadeiro sobre o problema**, por meio de fatos e regras. A linguagem utiliza mecanismos de inferência e busca para encontrar respostas que satisfaçam as relações especificadas pelo programa.

Assim, o programador não precisa indicar explicitamente uma sequência de passos equivalente àquela encontrada em uma linguagem imperativa.

### Exemplo simples

**Imperativo:**

> "Pegue X, compare X com Y, faça uma atribuição e repita enquanto determinada condição for verdadeira."

**Declarativo/Prolog:**

> "X e Y possuem determinada relação; estas são as regras que definem essa relação."