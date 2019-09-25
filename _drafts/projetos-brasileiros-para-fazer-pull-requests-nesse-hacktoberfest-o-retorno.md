---
title: 'Projetos Brasileiros para fazer pull requests nesse #Hacktoberfest o retorno'
layout: post
date: 2019-09-24T11:00:00.000+00:00
image: "/images/variados.png"
tags:
- pull request
- pull requests
- contribuitions
- open-source
- hacktoberfest
- GitHub
- Git
- open source
- português
comments: true
description: 'Versão 2019 da lista de projetos brasileiros para contribuir no #Hacktoberfest'

---
Depois dos sucessos das listas [de 2017](https://medium.com/nossa-coletividad/projetos-brasileiros-para-fazer-pull-requests-nesse-hacktoberfest-4dc9b9b576c0) e [de 2018](https://medium.com/@jessicatemporal/projetos-brasileiros-para-contribuir-nesse-hacktoberfest-vers%C3%A3o-2018-4925959b9411), esse é o terceiro ano que estou fazendo a lista/curadoria de projetos brasileiros para contribuir no #Hacktoberfest.

Então a pedidos aqui vai! Uma lista toda repleta de projetos pra você contribuir nesse mês de Outubro!

Novamente temos regrinhas:

1. Ser um projeto criado/desenvolvido/mantido por brasileiras(os);
2. Ter pelo menos uma issue aberta.

## Avisos para 2019

Essa lista **deve crescer** ao longo do mês de outubro e foi feita pra ser colaborativa… Então se sabe de um projeto que deveria estar aqui, só mandar o link que eu coloco, oooouuu você pode aproveitar o espírito de contribuição e mandar um PR para adicionar o projeto (eu vou liberar o guia de contribuição daqui um tempinho)! Todo mundo ganha <3.

Esse ano os projetos estão separados pela linguagem principal pra facilitar as buscas pra quem lê e também em ordem alfabética pela linguagem. Se quiser adicionar um projeto pra uma liguagem que não estiver na lista só se atentar para isso, beleza? 😉

E diferentementemente do ano passado! Essa lista agora não está mais no Medium \\o/

***

{% assign grouped = site.hacktoberfest_projects | group_by: "principal_language" %}
{% for group in grouped %}
<h2> {{ group.name }} </h2>
{% for item in group.items %}
 <div class="github-project-share">
 <a style="text-decoration: none;" href="{{ item.repo }}">
 {% assign project_info = item.relative_path |  remove: ".md" | remove: ".yml" | split: "/"  %}
 {% assign project = project_info[2] | replace: "+", "/" %}
 <div class="github-project-share-card ">
 <img src="{{ item.image }}" alt="" />
 <h4>{{ project }}</h4>
 <br/>
 <p>{{ item.description }}</p>
 <p><small>github.com</small></p>
 </div>
 </a>
 </div>
{%endfor%}

***

{%endfor%}