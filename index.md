---
layout: default
title: Início
---

<div class="intro" markdown="1">

# João Felipe

Notas sobre programação, projetos e coisas que estou aprendendo.

</div>

## Últimas notas

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">
      <span class="post-list-title">{{ post.title }}</span>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d/%m/%Y" }}</time>
    </a>
  </li>
{% endfor %}
</ul>
