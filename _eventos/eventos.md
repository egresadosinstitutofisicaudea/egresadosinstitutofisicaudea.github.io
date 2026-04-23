---
layout: archive
title: "Eventos"
permalink: /eventos/
---


---

## Próximos eventos

<div class="grid-eventos">

{% for e in site.eventos %}

<div class="card-evento">

  <h3>{{ e.title }}</h3>
  
  {% if e.excerpt %}
    <p>{{ e.excerpt }}</p>
  {% endif %}

  {% if e.image %}
    <img src="{{ e.image }}" style="width:40%; height:auto; border-radius:10px;">
  {% endif %}

  

</div>

{% endfor %}

</div>
