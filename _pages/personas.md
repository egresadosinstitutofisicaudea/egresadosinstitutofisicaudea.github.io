---
layout: archive
title: "Banco de egresados y egresadas"
permalink: /egresados/
---

Si quieres hacer parte de este banco contáctanos al correo egresadosinstitutofisicaudea@gmail.com

---

<div class="grid-personas">

{% for persona in site.egresados %}

<a href="{{ persona.url }}" style="text-decoration:none; color:inherit;">

  <div class="card-persona">

    <div class="nombre">{{ persona.nombre }}</div>

    {% if persona.formacion %}
      <div class="area">{{ persona.formacion }}</div>
    {% endif %}

    {% if persona.areas %}
      <div class="area">{{ persona.areas }}</div>
    {% endif %}

  </div>

</a>

{% endfor %}

</div>
