---
title: " "
permalink: /seção3/
layout: single
author_profile: false
mathjax: true
header:
  overlay_image: /assets/images/logos3.png
  actions:
    - label: "<br />Tutorial para o uso do software Insight Maker<br /> <small>Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit</small>"
      url: "/seção3/#lógica-de-funcionamento-do-software/"    
sidebar:
  title: " "
  nav: blogroll
mathjax: true
---
# Lógica de funcionamento do software


<div class="box">
  <small><span style="font-family: Comic Sans MS">teste</span> continuando do texto</small>
  <span></span>
  <span></span>
</div>

O _Insight Maker_ usa comandos no idioma inglês. Então, estoque é designado por _stock_ e fluxo por _flow_. Vamos traduzir na primeira vez em que a palavra inglesa for usada e depois usaremos indistintamente em português ou inglês.
{: .text-justify}

Na Figura 1.1 da <a href="https://milenalauschner.github.io/MM/seção1/">Seção 2</a> vê-se o que se chama de diagrama _stock-flow_. Um diagrama _stock-flow_  mostra uma parte da realidade que se pretende investigar através da criação de um sistema com componentes interligadas. No _Insight Maker_ essas componentes são chamadas de _primitives_ - em português primitivas. Uma das razões para que esses diagramas  sejam tão úteis na construção da aprendizagem é que conseguimos visualizar como uma primitiva individual impacta no coletivo do sistema, na acumulação que ocorre no estoque.
{: .text-justify}

Acumulações estão em todos os lugares em nossas vidas (CLExchange, 2016). Nesse primeiro momento estamos usando o exemplo de acumulação de livros em uma biblioteca, mas poderíamos nos preocupar com a acumulação de dinheiro depositado em uma conta de poupança, com a acumulação de água em um balde durante uma chuva, com a acumulação de velocidade das pedras de granizo que caem durante uma tempestade, etc.
{: .text-justify}

As acumulações são representadas por retângulos associados aos estoques, que podem variar pela existência de um fluxo, representado por uma seta com linha contínua. O fluxo é responsável por diminuir, aumentar ou manter constante o nível do estoque.
{: .text-justify}

Existem também componentes que podem influenciar no comportamento de um fluxo. São as chamadas variáveis (_variables_). Apesar do significado do nome, elas podem ser variáveis ou constantes. Por exemplo, no caso mais simplificado de uma biblioteca, vê-se na Figura 1.2 a existência de duas variáveis: uma que estipula um prazo de devolução para os livros e outra para representar a porcentagem de empréstimos feitos durante um período. A primeira variável vai impactar diretamente no fluxo de devoluções, pois, ao acabar o tempo que o aluno pode permanecer com o livro, ele deverá devolvê-lo à biblioteca. A criação da segunda variável mostrará como acontece a diminuição de livros na biblioteca.
{: .text-justify}

 ![Figura 1.2: Diagrama stock-flow da biblioteca com as variáveis.]({{ site.url }}{{ site.baseurl
}}/assets/images/BIBLIOTECA2.png){: .align-center}   

{: .image-caption}
*Figura 1.2: Diagrama stock-flow da biblioteca com as variáveis.*
 {: .text-center} 
 
Na Figura 1.2 também aparecem linhas pontilhadas que representam as ligações entre variável e fluxo. Essas ligações são denominadas _links_. Todas as variáveis do sistema são ligadas ao fluxo por meio de _links_. Os _links_ não servem estritamente para conectar variáveis aos fluxos, mas também podem indicar como um estoque influencia em outro ou como uma variável compõe outra variável. Ou seja, fazem ligações entre diferentes componentes.
{: .text-justify}
 
As componentes apresentadas até aqui são sintetizadas na Tabela 1.1.
{: .text-justify}

Tabela 1.1: Resumo dos componentes do diagrama _stock-flow_ 
{: .text-center}

|  Componente |                     Descrição                 |
|   :----:    |                      :----                   |   
|Estoque | Primitiva com formato retangular que representa as acumulações ocorridas num sistema.|        
| Fluxo  | Flecha com linha contínua que representa uma taxa de variação. Influencia nas acumulações podendo diminuir, aumentar ou manter constante o nível do estoque. |
|Variável| Primitiva de formato elipsoidal que influencia no comportamento do fluxo ou compõe  outras variáveis. Ela pode ser uma grandeza variável ou constante (parâmetros).| 
| _Links_|Flecha com linhas pontilhadas que servem como conectores entre variáveis, fluxos e estoques.|         

 Olhando para o diagrama _stock-flow_ da biblioteca com suas variáveis adicionadas (Figura 1.2), notamos que estão faltando componentes nesse modelo para ser uma representação mais realista de uma biblioteca em funcionamento. Os empréstimos geram acumulação de livros emprestados, por isso devemos criar um novo estoque (de livros emprestados). O fluxo de devoluções diminui o número de livros emprestados ao passo que o fluxo de empréstimos aumenta. Isso significa que os sentidos dos fluxos para esse novo estoque serão opostos aos dos fluxos do estoque de livros na biblioteca. A Figura 1.3 mostra o modelo construído para a biblioteca neste exemplo.
{: .text-justify} 

 ![Figura 1.3: Modelo da biblioteca.]({{ site.url }}{{ site.baseurl
}}/assets/images/BIBLIOTECA3.png){: .align-center}   
{: .image-caption}
*Figura 1.3: Modelo da biblioteca.*
 {: .text-center}
 
Esse modelo tem limitações decorrentes das seguintes idealizações assumidas:
{: .text-justify} 

  * o funcionamento da biblioteca ocorre nos sete dias da semana;
  * todos os livros retirados são devolvidos, ou seja, desconsidera-se não devolução de livros por qualquer motivo;
  * o prazo para devolução é constante, não dependendo do tipo de livro retirado;    
  * a porcentagem de empréstimo é constante, não dependendo do período letivo.
  {: .text-justify} 
  
Esse modelo poderia ser aprimorado, caso nosso interesse fosse em efetivamente descrever o funcionamento de uma biblioteca, por exemplo, incluindo o aumento de estoque com a compra de livros, disponibilidade de livros virtuais, ocorrência de não devolução de livros, variação do prazo de devolução conforme o tipo de livro, fechamento da biblioteca aos domingos. Porém nosso objetivo se resume a introduzir as principais ferramentas do _Insight Maker_ com um exemplo familiar, o de uma biblioteca. Então, vamos seguir com o modelo mais simples.
{: .text-justify} 

Vamos agora propor a seguinte situação-problema: uma avaliação sobre a utilização do acervo de livros das bibliotecas escolares está sendo feita pela Secretaria Municipal de Educação. Por isso, um bibliotecário quer fazer uma estimativa do número de livros que estarão disponíveis na biblioteca em determinada data, quando será feita a inspeção. Para isso ele começa apurando alguns dados.
{: .text-justify} 

Ele observa que:

  * em um determinado dia, do acervo total de 1450 livros, 1100 estavam no estoque da biblioteca no início do dia;
  * <div class="box">
  nesse dia foram emprestados 33 livros, ou seja, 3% do número de <span style="font-family: Comic Sans MS">Livros na biblioteca</span> continuando do texto. Como esse é um dia típico de funcionamento da biblioteca, ele assume que o fluxo diário de livros que saem da biblioteca é <span style="font-family: Comic Sans MS">Empréstimos</span>= <span style="font-family: Comic Sans MS">Porcentagem de empréstimos</span> multiplicado por <span style="font-family: Comic Sans MS">Livros na biblioteca</span>= 0,03 $$\cdot$$ <span style="font-family: Comic Sans MS">Livros na biblioteca</span>
    </div>
    
    nesse dia foram emprestados 33 livros, ou seja, 3$$\%$$ do número de < span style=”color:red;font-size:15px” > you< /span> < span style="font-family:Comic Sans MS">Livros na biblioteca< /span>. Como esse é um dia típico de funcionamento da biblioteca, ele assume que o fluxo diário de livros que saem da biblioteca é "Empréstimos"= "Porcentagem de empréstimos" multiplicado por <p style="font-family:Comic Sans MS">Livros na biblioteca</p>= 0,03 $$\cdot$$ <p style="font-family:Comic Sans MS">Livros na biblioteca</p>;
  * o número médio de devoluções de livros por dia é praticamente constante. Como o prazo de devolução é de 7 dias, ele assume que o fluxo de "Devoluções" diário é o número de "Livros emprestados" dividido pelo "Prazo de empréstimo"= "Livros emprestados"/7.
{: .text-justify} 

Feitas essas estimativas iniciais, se a inspeção ocorrerá dentro de 4 dias, não será muito trabalhoso o bibliotecário construir a Tabela 1.2.
{: .text-justify} 

*Tabela 1.2: Número de livros na biblioteca*
{: .text-center}

| dia| <p style="font-family:Comic Sans MS">Livros na biblioteca</p> no início do dia ($$n$$)| "Livros emprestados" no início do dia ($$m$$)|"Empréstimos" $$0,03$$ x $$n$$|Devoluções" $$m$$/$$7$$|
|:----:  |           :----:             |           :----:           |     :----:     |     :----:       |
| $$0$$  |         $$1100$$             |           $$350$$          |     $$33$$     |     $$50$$       |
| $$1$$  |         $$1117$$             |           $$333$$          |     $$34$$     |     $$48$$       |
| $$2$$  |         $$1131$$             |           $$319$$          |     $$34$$     |     $$46$$       |
| $$3$$  |         $$1143$$             |           $$307$$          |     $$34$$     |     $$44$$       |
| $$4$$  |         $$1153$$             |           $$297$$          |     $$35$$     |     $$42$$       |



Como ele construiu essa tabela? 

Na primeira linha ele colocou os valores iniciais das grandezas, ou seja:
{: .text-justify} 

  * dia = 0
  * número de <p style="font-family:Comic Sans MS">Livros na biblioteca</p> no início do dia = 1100, pois é o número de livros que ele contou no início do dia;
  * número de "Livros emprestados" = 350, já que o acervo da biblioteca é 1450, há 1100 na biblioteca e ele está assumindo que não houve extravios. De fato, ele confere o número de empréstimos e verifica que há 350 emprestados;
  * em um determinado dia, do acervo total de 1450 livros, 1100 estavam no estoque da biblioteca no início do dia;
  * número de empréstimos = 33, pois o número de empréstimos diários é 0,03 $$\cdot$$ <p style="font-family:Comic Sans MS">Livros na biblioteca</p> e nesse dia há  1100 livros na biblioteca. Então, 0,03 $$\cdot$$ 1100 = 33;
  * número de devoluções = 50, pois o número de devoluções diárias é "Livros emprestados"/7 e nesse dia há 350 livros emprestados. Então, 350/7 = 50.   
{: .text-justify} 

Na segunda linha os estoques de livros na biblioteca e emprestados deverão ser atualizados de acordo com os fluxos de entrada e saída de livros, ou seja, com o número de livros emprestados e devolvidos. Então:
{: .text-justify} 

  * dia = 1
  * número de <p style="font-family:Comic Sans MS">Livros na biblioteca</p> no início do dia é o número que havia no dia anterior, menos o que foi emprestado ao longo do dia anterior mais o que foi devolvido ao longo do dia anterior. Então, é: 1100 - 33 + 50 = 1117. Podemos escrever como:
{: .text-justify} 

<p style="font-family:Comic Sans MS">Livros na biblioteca</p> (dia = 1) = <br />
<p style="font-family:Comic Sans MS">Livros na biblioteca</p>  (dia = 0) - "Empréstimos" (dia = 0) + "Devoluções"(dia = 0);
{: .text-center} 

* número de "Livros emprestados" no início do dia: número que estava emprestado no dia anterior mais o que foi emprestado ao longo do dia anterior menos o que foi devolvido = 350 + 33 - 50 = 333. Podemos escrever como: 
{: .text-justify} 

"Livros emprestados"(dia = 1) =<br />
"Livros emprestados" (dia = 0) + "Empréstimos"(dia = 0) - "Devoluções" (dia = 0);
{: .text-center} 

* número de empréstimos = 34, pois o número de empréstimos diários é 0,03 $$\cdot$$ <p style="font-family:Comic Sans MS">Livros na biblioteca</p> e nesse dia há  1117 <p style="font-family:Comic Sans MS">Livros na biblioteca</p>. Então, 0,03 $$\cdot$$ 1117 = 33,51. Isso fica expresso como:
{: .text-justify} 

"Empréstimos"(dia = 1) = "Porcentagem de empréstimos" $$\cdot$$ <p style="font-family:Comic Sans MS">Livros na biblioteca</p>(dia = 1);  
{: .text-center} 

* número de devoluções = 48, pois o número de devoluções diárias é "Livros emprestados"/ 7 e nesse dia há 333 livros emprestados. Então, 333/7 = 47,57.  Ou seja,
{: .text-justify} 

 "Devoluções" (dia = 1) = "Livros emprestados"(dia = 1)/"Prazo de empréstimos". 
{: .text-center} 

Opa, não faz sentido valor fracionário para o número de livros, então, o número 33,51 e 47,57 foram arredondados na Tabela 1.2, para 34 e 48, que são os números inteiros mais próximos.   
{: .text-justify} 

Esse é um detalhe muito importante: só faz sentido trabalhar com números inteiros (e positivos)
de livros. Sempre que os cálculos produzirem valores fracionários, é preciso arredondar para o
inteiro mais próximo.
{: .text-justify} 

Podemos sintetizar os cálculos que o bibliotecário precisa fazer para completar a tabela do
seguinte modo:
{: .text-justify} 

<p style="font-family:Comic Sans MS">Livros na biblioteca</p> (dia = n+1) =<br />
<p style="font-family:Comic Sans MS">Livros na biblioteca</p> (dia = n) - "Empréstimos" (dia = n) + "Devoluções" (dia = n). 
{: .text-center} 

De modo semelhante: 

"Livros emprestados"(dia = n+1) =<br />
"Livros emprestados" (dia = n) + "Empréstimos" (dia = n) - "Devoluções" (dia = n). 
{: .text-center} 

E ainda: 

"Empréstimos"(dia = n) = "Porcentagem de empréstimos" $$\cdot$$ <p style="font-family:Comic Sans MS">Livros na biblioteca</p> (dia = n). <br />
e <br />
"Devoluções"(dia = n) =  "Livros emprestados" (dia = n)/ "Prazo de empréstimos"
{: .text-center}  

Em síntese as respostas produzidas pelo bibliotecário são: o número de <p style="font-family:Comic Sans MS">Livros na biblioteca</p> no quarto dia é 1153 e o porcentual de "Livros emprestados" é 297 $$\cdot$$ 100$$\%$$/1450, ou seja, aproximadamente 20$$\%$$.
{: .text-justify} 

Não é difícil fazer esses cálculos, mas se a inspeção ocorresse dentro de um mês ou mesmo dentro de meio ano, o bibliotecário teria bem mais trabalho para resolver o problema.
{: .text-justify} 

Vamos, então, deixar que o _Insight Maker_ faça a simulação do número de livros na biblioteca em função do tempo. 
{: .text-justify} 

## Referências
 [3] _CLExchange. Introduction to System Dynamics Models_ (2016).<br />
<a href="https://www.youtube.com/watch?v=IenySRdkRu8">https://www.youtube.com/watch?v=IenySRdkRu8</a>
{: .text-left}

[<i class="fas fa-arrow-alt-circle-left"></i> Seção 2](https://milenalauschner.github.io/MM/seção2/){:
.btn .btn--success}[ Seção 4 <i class="fas fa-arrow-alt-circle-right"></i>](https://milenalauschner.github.io/MM/seção4/){:
.btn .btn--danger}
{: .text-right} 
________________________________________________________________________________________________________________________________________________________________________________________________
