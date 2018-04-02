---
layout: layout
title: "Eventos Futuros"
---

<section class="content">

Eventos Futuros
===============

**2018-1**

Aquí se encuentran algunos de los futuros eventos del comite interno de
ingeniería matematica.

<ul class="listing">
  {% assign upcoming = (site.posts | where: "category" , "upcoming") %}
  {% for post in upcoming reversed %}
  <li>
  <span>{{ post.date | date: "%B %e, %Y" }}</span> <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>
</section>
