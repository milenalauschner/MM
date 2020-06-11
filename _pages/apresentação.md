---
title: "Apresentação"
permalink: /apresentação/
layout: single
author_profile: false
header:
  image: /assets/images/header.png
sidebar:
  title: "Sumário"
  nav: blogroll
---
Este é um caderno de estudo sobre a modelagem de eventos físicos com o uso do _Insight Maker_.  O _Insight Maker_ é um _software_ para o estudo de sistemas dinâmicos, disponível livremente na _web_, podendo ser rodado _on-line_ a partir do endereço https://insightmaker.com. Nesse _software_ é possível simular sistemas dinâmicos simples ou bem complicados, sem precisar utilizar equações para resolver os problemas. Isso é possível porque os modelos são construídos usando somente diagramas.
{: .text-justify}

Essa possibilidade de representação de uma situação real ou abstrata como um sistema complexo revelando a conexão entre suas partes componentes, por meio somente de diagramas, é característica de um tipo específico de modelagem chamada Dinâmica de Sistemas e fundada pelo Prof. Jay Forrester do MIT Sloan School of Management (Sterman, 2016).
{: .text-justify}

Neste caderno vamos responder questões sobre sistemas ou eventos físicos, de preferência do nosso cotidiano, partindo de algum representação simplificada desse sistema. 
{: .text-justify}

Para facilitar a compreensão do funcionamento do _Insight Maker_, vamos descrever a lógica de construção de modelos neste _software_, e as suas principais características, nos valendo de um exemplo comum na vida de um estudante: uma biblioteca com uma coleção de livros que são cedidos por empréstimo aos estudantes da escola.
{: .text-justify}

Vamos querer responder questões do tipo: 

  * Quantos livros permanecem na biblioteca depois de certo tempo? 

Para isso vamos construir um modelo sobre o estoque de livros na biblioteca levando em conta que há empréstimos e devoluções. Como todo modelo, ele não representa exatamente o sistema em estudo. Trata-se de uma representação simplificada do sistema real, que poderá ser aprimorada na medida dos nossos interesses e conhecimentos sobre o sistema em estudo. 
{: .text-justify}

Considere que há certa quantidade de livros disponíveis em uma biblioteca, ou seja, tem um estoque de livros. Digamos que em certo momento haja $n$ livros na biblioteca. Essa quantidade de livros pode diminuir porque alguns livros são emprestados aos alunos, assim como pode aumentar porque alguns livros que estavam emprestados são devolvidos. Um diagrama que representa o número de livros na biblioteca está representado na Figura 1. Nessa figura, o retângulo representa o estoque de livros. As setas representam livros que entram ou saem da biblioteca.  A seta da esquerda, apontando para dentro do retângulo, indica que há um fluxo de livros entrando no estoque da biblioteca (devoluções de livros pelos alunos). A da direita, apontando para fora do retângulo, indica que há um fluxo de livros saindo do estoque da biblioteca (empréstimos de livros para alunos).
{: .text-justify}

  
  <figure class="align-center">
  <img src="/assets/images/biblioteca1.png" alt="Figura 1: Diagrama stock-flow da biblioteca.">
  <figcaption>Figura 1: Diagrama stock-flow da biblioteca.</figcaption>
</figure>

