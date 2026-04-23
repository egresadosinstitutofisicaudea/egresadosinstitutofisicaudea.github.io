---
layout: archive
title: "Eventos"
permalink: /eventos/
---

# Bienvenidos a la sección de eventos

Aquí encontrarás seminarios, charlas y actividades académicas del instituto.

![Imagen de eventos](/images/conversatorioEuropa.png)

---

<div class="grid-eventos">

{% for e in site.eventos %}

<div class="card-evento">

  <h3>{{ e.title }}</h3>

  {% if e.image %}
    <img src="{{ e.image }}" style="width:100%; border-radius:10px;">
  {% endif %}

  <p>{{ e.excerpt }}</p>

</div>

{% endfor %}

</div>
