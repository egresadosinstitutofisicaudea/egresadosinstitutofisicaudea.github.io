---
layout: archive
title: "Banco de egresados y egresadas"
permalink: /egresados/
---

Si quieres hacer parte de este banco contáctanos al correo egresadosinstitutofisicaudea@gmail.com


<div class="grid-personas">

{% for persona in site.data.personas %}

<div class="card-persona">

  <div class="nombre">{{ persona.nombre }}</div>

  {% if persona.formacion %}
  <div class="area">{{ persona.formacion }}</div>
  {% endif %}

  {% if persona.areas %}
  <div class="area">{{ persona.areas }}</div>
  {% endif %}

  <div style="margin-top:10px;">
    {% for p in persona.programas limit:2 %}
      <div class="programa">
        <strong>{{ p.tipo }}</strong> – {{ p.lugar }}
      </div>
    {% endfor %}
  </div>

  <div style="margin-top:8px;">
    {% for p in persona.programas %}
      <span class="tag">{{ p.tipo }}</span>
    {% endfor %}
  </div>

  <div style="margin-top:12px;">
    {% if persona.email %}
      <a href="mailto:{{ persona.email }}">📧 Contactar</a>
    {% endif %}
  </div>

</div>

{% endfor %}

</div>
