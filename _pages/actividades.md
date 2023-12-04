---
title: Actividades
permalink: "/actividades/"
author_profile: true
sitemap: false
classes: wide
---

{% assign actividades = site.actividades | reverse %}


{% for activity in actividades %}
<div class="container m-2">
  <div class="d-flex flex-wrap">
  <div class="card">
    <div class="row g-0">
        <div class="col-md-4">
        <a href="{{activity.link}}" title="Go to URL" target="_blank"><img src="{{activity.logo}}" class="card-img" alt="{{activity.name}}"></a>
        </div>
    <div class="col-md-8">
        <div class="card-body">
        <h6 class="card-title">{{activity.name}}</h6>
        <p class="card-text" style="font-size: 0.7rem;">{{activity.description}}</p>
        {% if activity.fecha %}
        <p class="card-text" style="font-size: 0.6rem;"><em>Fecha y lugar: {{activity.fecha}}</em></p>
        {% endif %}
        {% if activity.organizers %}
        <p class="card-text" style="font-size: 0.6rem;"><em>Organizadores: {{activity.organizers}}</em></p>
        {% endif %}
        </div>
    </div>
  </div>
  </div>
  </div>
</div>
{% endfor %}
  