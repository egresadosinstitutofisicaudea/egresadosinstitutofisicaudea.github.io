

<div class="grid-eventos">

{% for e in site.eventos %}

<a href="{{ e.url }}" style="text-decoration:none; color:inherit;">

<div class="card-evento">

  <h3>{{ e.title }}</h3>

  {% if e.excerpt %}
    <p><strong>{{ e.excerpt }}</strong></p>
  {% endif %}

  {% if e.image %}
    <img src="{{ e.image }}"
         style="width:100%; height:auto; border-radius:10px; margin-top:10px;">
  {% endif %}

</div>

</a>

{% endfor %}

</div>
