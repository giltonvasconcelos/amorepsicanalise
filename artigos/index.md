---
title: Artigos & Reflexões
layout: default
---

# Artigos & Reflexões

{% for artigo in site.artigos %}
<div class="card-artigo">
    <h2><a href="{{ artigo.url }}">{{ artigo.title }}</a></h2>
    <p class="data">{{ artigo.date | date: "%d/%m/%Y" }}</p>
    <p>{{ artigo.excerpt | default: "Clique para ler o artigo completo" }}</p>
</div>
{% endfor %}
