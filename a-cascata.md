# A cascata (cascading)

A escolha do browser de qual regra aplicar, caso haja muitas regras para o mesmo elemento.

* Seu estilo é lido de cima para baixo

É levado em considereção 3 fatores:

1 Origem do estilo
2 Especificidade
3 Importancia

### Origem do estilo

inline > tag style > tag link

### Especificidade

É um cálculo matemático onde cada tipo de seletor e origem do estilo, possuem valores a serem considerados.

<!-- Força de 0-->
0. Universal selector, combinators e negation pseudo-class (:not())

<!-- Força de 1-->
1. Element type selector e pseudo-elements (::before, ::after)

<!-- Força de 10-->
10. Classes e attribute selectors ([type="radio"])

<!-- Força de 100-->
100. ID selector

<!-- Força de 1000-->
1000. Inline

<!-- Força maior-->
### A regra !important

* cuidado, evite o uso
* não é considerado uma boa prática
* quebra o fluxo natural da cascata