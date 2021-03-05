# Seletores

## Selectors

Conecta um elemento HTML com o CSS a fim de alterar o elemento

### tipos

- Element sector
  - todos os elementos HTML
- ID Selector
  - Um elemento que tenha um atributo `id`.
  - Cada id deverá ser único.
- Class Selector
  - Os elementos que contenham um atributo `class`.
  - Podemos ter uma ou mais classes.
- Atribute selector
  - Um elemento que tenha um atributo específico.
- Pseudo-class selector
  - Elementos em um estado específico

## Combinators

Combinadores, pois else trabalham para buscar e combinar seletores a fim de aplicar uma estilização

### Descendant combinator

- Identificado por um espaço entre os seletores
- Busca um elemento dentro de outro

~~~~css
body article h2
~~~~

### Child combinator

- identificado pelo sinal `>` entre dois seletores.
- seleciona sempre o elemento que é filho direto do pai
- elementos depois do filho direto serão desconsiderados

~~~~css
body > ul > li
~~~~

### Adjacent sibling combinator

- Identificado pelo sinal `+` entre dois seletores
- Seleciona somente o elemnto do lado direito que é irmão direto na hierarquia

~~~~css
h1 + p
~~~~

### General sibling combinator

- identificado pelo sinal `~` entre dois seletores
- seleciona todos os elementos irmãos

~~~~css
h1 ~ p
~~~~

### Utilizando combinadores

~~~~css
ul > li[class="red"]
~~~~

## Dica

- Seletores muito específicos tendem a causar dificuldades no reuso das regras de estilização dos elementos
- Muitas vezes, um simples uso de classes, torna o trabalho muito mais eficiente.

## Pseudo-classes

É um tipo de seletor que irá selecionar um elemento que estiver em um estado específico.

Exemplo: É o primeiro elemento dentro de uma caixa, ou, o elemento está com ponteiro de mouse em cima dele.

Pseudo-classes começam com 2 pontos seguidos do nome da pseudo class
`:pseudo-class-name`

### Seleciona elementos com pseudo classes

- :first-child
- :nth-of-type()
- :nth-child()

## Ações do usuário

- :hover
- :focus

## Atributos

- :disabled
- :required

## Pseudo-elements

Com pseudo-elements nós podemos adicionar elementos HTML pelo próprio CSS

`::pseudo-element-name`

### Exemplo

- :: before
- :: after
- :: first-line
