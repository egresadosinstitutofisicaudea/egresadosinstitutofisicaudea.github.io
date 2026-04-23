---
layout: archive
title: "Eventos"
permalink: /eventos/
---

Bienvenidos a la sección de eventos.  
Aquí encontrarás seminarios, charlas y actividades académicas del instituto.

<!-- BANNER (sin recorte, solo escala) -->
<img src="/images/conversatorioEuropa.png"
     style="width:50%; height:auto; border-radius:12px; margin:20px 0;">

---

## Próximos eventos

<div class="grid-eventos">

{% for e in site.eventos %}

<div class="card-evento">

  <h3>{{ e.title }}</h3>

  {% if e.image %}
    <img src="{{ e.image }}"
         style="width:100%; height:auto; border-radius:10px; margin-bottom:10px;">
  {% endif %}

  {% if e.excerpt %}
    <p>{{ e.excerpt }}</p>
  {% endif %}

</div>

{% endfor %}

</div>
