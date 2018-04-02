---
layout: layout
title: "About"
---

<!-- You can edit this whole page, remove it, or use it as basis for any non-post pages you have. -->
<section class="content">

# {{ site.name }}

<ul class="listing">
<li>
<span>Semestre 2018-1</span><a href="{{ site.url }}/upcoming.html">Futuros eventos</a>
</li>
  {% assign upcoming = (site.posts | where: "category" , "upcoming") %}
  {% for post in upcoming reversed %}
    {% if forloop.first %}
    <li style="text-indent: 2em;">
    <span>{{ post.date | date: "%B %e, %Y" }}</span> Siguiente evento: <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endif %}
  {% endfor %}
<li>
<span>2017-2018</span><a href="{{ site.url }}/previous.html">Eventos previos</a>
</li>
</ul>

### Alguna descripción Cool
</section>
