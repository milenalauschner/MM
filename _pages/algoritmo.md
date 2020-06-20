---
title: " Algoritmo de análise"
title-color: #87c0cd
permalink: /algoritmo/
layout: single
author_profile: false
mathjax: true
header:
  image: /assets/images/header.png
sidebar:
  title: "Sumário"
  nav: blogroll
---

Uma vez que o modelo  já está implementado no _Insight Maker_ e já se atribuiu valores iniciais aos estoques, fluxos e variáveis, podemos observar como o sistema dinâmico evolui com o tempo. 
{: .text-justify}

  Para gerar um gráfico, é necessário clicar em _Settings_ e aparecerá uma janela como mostrado na Figura 7. É necessário definir o tempo inicial e final da simulação em _Simulation Start/ Simulation Length_ e a unidade do tempo (_Time Units_).  No presente caso usaremos dias (_days_) com a unidade de tempo.
{: .text-justify}

![Figura 7: Visualização da configuração da simulação.]({{ site.url }}{{ site.baseurl
}}/assets/images/SIMULAR.png){: .align-center}   

{: .image-caption}
*Figura 7: Visualização da configuração da simulação.*
 {: .text-center}
 
O método de integração pode ficar no valor de _default_, Método de Euler. Esse é o método que o bibliotecário utilizou para construir a Tabela 2, mesmo sem ter noção sobre métodos de integração. O Método de Euler é o método de integração mais simples que existe, bastante intuitivo, e que serve para muitos propósitos. 
{: .text-justify}

 Clica-se em _Apply_ e a simulação está pronta para ser rodada clicanco em _Simulate_. 
{: .text-justify}
 
 Os resultados são mostrados na forma de gráficos ou tabelas. Por exemplo, na Figura 8 são mostrados os valores obtidos para o número de "Livros na bibliotecas" e de "Livros emprestados" nos dias $0, 1, 2, 3...$, além do "Prazo de devolução" e da "Porcentagem de empréstimos" que são constantes. 
{: .text-justify}
 
 ![Figura 8: Valores obtidos para diversas grandezas do nosso modelo.]({{ site.url }}{{ site.baseurl
}}/assets/images/TABELA_FRAC.png){: .align-center}   

{: .image-caption}
*Figura 8: Valores obtidos para diversas grandezas do nosso modelo.*
 {: .text-center}
 
No entanto, estamos com um problema, pois o número de livros deve ser inteiro! Cometemos um equívoco no modelo e precisamos consertá-lo: precisamos impor que os valores obtidos para número de livros sejam inteiros. Para isso, vamos retornar às funções que definem os estoques e usar a função matemática Round, conforme mostrado na Figura 9.
{: .text-justify}
 
![Figura 9: Aplicação do arrendondamento nas equações.]({{ site.url }}{{ site.baseurl
}}/assets/images/ROUND.png){: .align-center}   

{: .image-caption}
*Figura 9: Aplicação do arrendondamento nas equações.*
 {: .text-center}
 
  Agora sim, rodando essa versão do modelo reproduzimos os valores obtidos pelo bibliotecário. 
{: .text-justify}
 
 Também podemos gerar gráficos. Por exemplo, a Figura 10 mostra um gráfico do número de livros em função do tempo para a biblioteca de nosso exemplo.
{: .text-justify}
 
 
 ![Figura 10]({{ site.url }}{{ site.baseurl
 }}/assets/images/BIBLIOTECA4.png){: .align-center}   

{: .image-caption}
*Figura 10: Gráfico de livros versus tempo.*
 {: .text-center}
 
 
 
 
