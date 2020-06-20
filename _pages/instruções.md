---
title: "Instruções para construir o seu modelo no Insight Maker"
permalink: /instruções/
layout: single
author_profile: false
mathjax: true
header:
  image: /assets/images/header.png
sidebar:
  title: "Sumário"
  nav: blogroll
---
O primeiro passo é criar uma conta livre na página do programa <a href="https://insightmaker.com">https://insightmaker.com</a>. Para isso basta entrar na opção _Create a free account_, no canto superior da página, e preencher algumas informações no formulário que se abrirá. Uma dessas informações é sua conta de email e uma senha de sua escolha. Então, acesse o login, no canto superior direito da página, para entrar na área de criação de modelos, e prossiga com as orientações abaixo.
{: .text-justify}

Clique em _Create New Insight_ (no canto superior direito) e, então, em _Click me to clear this Demo Model_ (no canto superior direito). Agora você tem à sua disposição a área para criação de modelos. 
{: .text-justify}

Para implementar o modelo mostrado na Figura 3 adicione os estoques do modelo usando o comando _Add primitive_ (topo esquerdo da tela do computador), e opte por _Add Stock_. Crie um estoque para os "Livros na biblioteca" e outro para os "Livros emprestados". Mova os retângulos que representam os estoques para a região da tela que julgar mais conveniente. Note que com o cursor em cima do retângulo, você vê uma setinha azul no meio do retângulo, e um sinal de igual no centro de uma bolinha cinza do lado esquerdo. Esses sinais lhes serão muito úteis. 
{: .text-justify}

Observe também que no topo da tela vê-se a Figura 4. A cor cinza indica que  é o comando _Flows_ que está ativo. Clicando em _Links_, ficará cinza, e será possível criar um  _link_. Clicando nas setinhas à direita se pode inverter o sentido de fluxos.
{: .text-justify}

![Figura 4: Comandos para a criação de fluxos e links.]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOW-LINKS.png){: .align-center}   

{: .image-caption}
*Figura 4: Comandos para a criação de fluxos e links.*
 {: .text-center} 
 
Clicando duas vezes sobre o retângulo você pode atribuir os nomes dos estoques: por ex., "Livros na biblioteca". Com o cursor em cima do estoque de "Livros na biblioteca", estenda a setinha azul para criar o fluxo que representa os empréstimos diários, ou seja, que vai do estoque de "Livros na biblioteca" para o estoque "Livros emprestados".  Faça o mesmo para criar o outro fluxo no sentido inverso. 
{: .text-justify}

Novamente em _Add primitive_, opte por _Add variables_ para criar as variáveis "Prazo para devolução" e "Porcentagem de empréstimos". Finalmente,  clique em _Links_, para criar o _link_ entre cada variável e o fluxo que ela influenciará. 
{: .text-justify}

Você deve ter conseguido reproduzir a Figura 3. Resta agora introduzir as equações que relacionam essas grandezas, assim como os valores iniciais. 
{: .text-justify}

Já vimos que o fluxo de "Devoluções" é igual a "Livros emprestados" dividido pelo valor da variável "Prazo de devolução", que tomaremos igual a $$7$$. 
{: .text-justify}

Para introduzir essas informações no modelo, basta proceder como mostrado na Figura 5. 
{: .text-justify}

 ![Figura 5: Visualização da criação de fluxos.]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOW.png){: .align-center}   

{: .image-caption}
*Figura 5: Visualização da criação de fluxos.*
 {: .text-center}
 
Já o fluxo de livros que sai da biblioteca ("Empréstimos") será igual ao valor do estoque de "Livros na biblioteca" vezes o valor da variável "Porcentagem de empréstimos".  Para introduzir essas informações no modelo, basta proceder como mostrado na Figura 6. 
{: .text-justify}
 
 ![Figura 6: Visualização da criação de fluxos.]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOW2.png){: .align-center}   

{: .image-caption}
*Figura 6: Visualização da criação de fluxos.*
 {: .text-center}
 
 Vamos agora inserir o valor $$0.03$$ para a variável "Porcentagem de empréstimos". Para isso, clique em cima do diagrama dessa variável, abre-se uma janela onde você preencherá ao lado de _Value/Equation_ o valor $$0.03$$. Note  que no _Insight Maker_ é usado ponto para separar as casas decimais, não vírgula. Cuidado para não utilizar vírgula!
{: .text-justify}

Resta colocar o valor inicial nos estoques. Clique em cima do retângulo que representa cada estoque e coloque o número inicial de "Livros na biblioteca" igual à "$$1100$$" e valor inicial de "Livros emprestados" igual à $$440$$.
{: .text-justify}

[Seção 2](https://milenalauschner.github.io/MM/funcionamento/){:
.btn .btn--success}

 
