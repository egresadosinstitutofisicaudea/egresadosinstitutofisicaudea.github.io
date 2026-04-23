---
layout: archive
title: "Eventos"
permalink: /eventos/
---

# Bienvenidos a la sección de eventos

Aquí encontrarás seminarios, charlas y actividades académicas del instituto.

<img src="/images/conversatorioEuropa.png"
     style="width:100%; max-height:300px; object-fit:cover; border-radius:12px;">

---

## Próximos eventos

<div class="grid-eventos">

{% for e in site.eventos %}

<div class="card-evento">

  <h3>{{ e.title }}</h3>

  {% if e.image %}
    <img src="{{ e.image }}" style="width:100%; height:200px; object-fit:cover; border-radius:10px;">
  {% endif %}

  {% if e.excerpt %}
    <p>{{ e.excerpt }}</p>
  {% endif %}

</div>

{% endfor %}

</div>
