---
title: "  "
layout: single
datatable: true
permalink: /about/
author_profile: false
header:
  overlay_color: "#5e616c"
  image: /assets/images/logos.png
  actions:
    - label: " Universidade Federal do Rio Grande do Sul<br /> Instituto de Física<br />  <small>Tutorial para o uso do software Insight Maker</small><br /> Autores: Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit ______________________________________________________________________________________________________________________"
sidebar:
  title: "Sumário"
  nav: blogroll
---
{% include feature_row id="intro" type="center" %}
<style type="text/css">
  .main-container {
  max-width: 1800px;
  margin-left: auto;
  margin-right: auto;
}
</style>

<!-- This loops through the paginated posts -->
{% for post in paginator.posts %}
  <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
  <p class="author">
    <span class="date">{{ post.date }}</span>
  </p>
  <div class="content">
    {{ post.content }}
  </div>
{% endfor %}

<!-- Pagination links -->
<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}" class="previous">
      Previous
    </a>
  {% else %}
    <span class="previous">Previous</span>
  {% endif %}
  <span class="page_number ">
    Page: {{ paginator.page }} of {{ paginator.total_pages }}
  </span>
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" class="next">Next</a>
  {% else %}
    <span class="next ">Next</span>
  {% endif %}
</div>
Instituto de Física <br/> 
Tutorial online sobre o uso do software Insight Maker <br/> 
Autores: Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit"

|                	| Tutorial sobre o uso do software Insight Maker|                	|
|:----:           |                  :----:	                   |      :-----:   	|
|![UFRGS]({{ site.url }}{{ site.baseurl}}/assets/images/UFRGS.png){: .align-center}|Autores: Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit|![IF]({{ site.url }}{{ site.baseurl}}/assets/images/IF.png){: .align-center}|
||||


> title: Universidade Federal do Rio Grande do Sul
excerpt: "Instituto de Física <br/> Tutorial sobre o uso do software Insight Maker <br/> Autores: Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit"
> header:
  overlay_color: $background-color
> open-source software.

[<i class="fas fa-file-pdf"></i> See my
Résumé](https://ln2.sync.com/dl/37ab0c9b0/pu7bvjv3-9gv6sjie-ggmayp6u-jy8jr59r){:
.btn .btn--info .btn--default}

![Black-and-white photo of George smiling while sitting cross legged and
brushing his hair]({{ site.url }}{{ site.baseurl
}}/assets/images/portrait.jpg){: .align-center}

Hello! My name is George.

I'm a financial data scientist and machine learning researcher, with a focus on
Bayesian modelling and probabilistic programming. I'm based in New York and I
work for [Point72 Asset Management](http://point72.com).

In my ~~copious~~ free time, I contribute to and maintain [several open-source
libraries](https://eigenfoo.xyz/work/#software) (particularly the [PyMC
project](https://github.com/pymc-devs)). Away from the keyboard, I spend my time
drinking coffee, taking photos and obsessing over [mechanical
keyboards](https://www.reddit.com/r/MechanicalKeyboards/),
[headphones](https://www.reddit.com/r/headphones/) and [fountain
pens](https://www.reddit.com/r/fountainpens/).

Previously, I studied engineering at [The Cooper
Union](http://cooper.edu/welcome) with minors in computer science and
mathematics, and I interned at [Quantopian](https://www.quantopian.com/) on
their quant research and data science teams.

## What's with your username?

It seemed clever at the time... but people keep asking, so maybe not.

_Eigen_ is a German for _own_, but probably a better translation (especially for
math terms like
[eigenvalue](https://en.wikipedia.org/wiki/Eigenvalues_and_eigenvectors)) would
be _belonging to_. For example, an eigenvalue is the value _belonging to_ a
matrix.

_Foo_ is a [placeholder name in computer
programming](https://en.wikipedia.org/wiki/Foobar), and is basically a techier
version of "stuff" or "thing".

So on one hand, my username is unique and belongs to me because its `eigen`, but
on the other hand its just a `foo`. The juxtaposition was funny to me.
