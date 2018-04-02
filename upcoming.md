---
layout: layout
title: "Eventos Futuros"
---

<section class="content">

Futuros Eventos
===============

Aquí se encuentran algunos de los futuros eventos del comite interno de
ingeniería matematica.

**2018-1**

<ul class="listing">
  {% assign upcoming = (site.posts | where: "category" , "upcoming") %}
  {% for post in upcoming reversed %}
  <li>
  <span>{{ post.date | date: "%B %e, %Y" }}</span> <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>
</section>
