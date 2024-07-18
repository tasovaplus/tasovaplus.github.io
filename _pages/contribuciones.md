---
title: Contribuciones
permalink: "/contribuciones/"
author_profile: true
sitemap: false
classes: wide
---

{% assign contribuciones = site.contribuciones | reverse %}


{% for contribution in contribuciones %}
<div class="container m-2">
  <div class="d-flex flex-wrap">
  <div class="card">
    <div class="row g-0">
    <div class="col-md-12">
        <div class="card-body">
        <h6 class="card-title">{{contribution.name}}</h6>
        <p class="card-text" style="font-size: 0.7rem;">{{contribution.description}}</p>
        </div>
    </div>
  </div>
  </div>
  </div>
</div>
{% endfor %}