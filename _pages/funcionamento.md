---
title: "Lógica de funcionamento do software"
permalink: /funcionamento/
layout: single
author_profile: false
mathjax: true
classes: wide
header:
  image: /assets/images/header.png
sidebar:
  title: "Sumário"
  nav: blogroll
---

O _Insight Maker_ usa comandos no idioma inglês. Então, estoque é designado por _stock_ e fluxo por _flow_. Passaremos a usá-los indiferentemente na denominação em inglês ou português.
{: .text-justify}

Na Figura 1 vê-se o que se chama de diagrama _stock-flow_. Um diagrama _stock-flow_  mostra uma parte da realidade que se pretende investigar através da criação de um sistema com componentes interligadas. No _Insight Maker_ essas componentes são chamadas de _primitives_ - em português primitivas. Uma das razões para que esses diagramas  sejam tão úteis na construção da aprendizagem é que conseguimos visualizar como uma primitiva individual impacta no coletivo do sistema, na acumulação que ocorre no estoque.
{: .text-justify}

Acumulações estão em todos os lugares em nossas vidas. Nesse primeiro momento estamos usando o exemplo de livros em uma biblioteca, mas poderíamos nos preocupar com o dinheiro depositado em uma conta de poupança, com a acumulação de água em um balde durante uma chuva, com a  acumulação de velocidade das pedras de granizo que caem durante uma tempestade, etc.
{: .text-justify}

As acumulações são representadas por retângulos associados aos estoques, que podem variar pela existência de um fluxo, representado por uma seta com linha contínua. O fluxo é responsável por diminuir, aumentar ou manter constante o nível do estoque.
{: .text-justify}

Existem também componentes que podem influenciar no comportamento de um fluxo. São as chamadas variáveis _variables_. Apesar do significado do nome, elas podem ser variáveis ou constantes. Por exemplo, no caso mais simplificado de uma biblioteca, vê-se na Figura 2 a existência de duas variáveis, uma para estipular um prazo de devolução dos livros e outra para representar a porcentagem de empréstimos feitos durante um período. A primeira variável vai impactar diretamente no fluxo de devoluções, pois ao acabar o tempo que o aluno pode permanecer com o livro ele deverá devolver à biblioteca. A  criação da segunda variável mostrará de forma mais clara como acontece a diminuição de livros na biblioteca.
{: .text-justify}
