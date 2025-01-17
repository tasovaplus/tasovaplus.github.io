---
title: Herramientas

permalink: "/herramientas/"
author_profile: true
sitemap: false
classes: wide
---

{% assign tools = site.tools | sort: "number" %}

<div class="container">
  <div class="d-flex flex-wrap">
{% for tool in tools %}
<div class="p-2">
  <div class="card"  style="width: 12rem;">
    <img src="{{tool.logo}}" class="card-img-top" alt="{{tool.name}}">
    <div class="card-body">
      <h6 class="card-title">{{tool.name}}</h6>
      <p class="card-text" style="font-size: 0.7rem;">{{tool.description}}</p>
      <p class="card-text" style="font-size: 0.6rem;"><em>Autores: {{tool.authors}}</em></p>
      <a href="{{tool.link}}" target="_blank" title="Go to URL"><i class="bi bi-box-arrow-up-right"></i></a>
        <a href="{{tool.doi}}" target="_blank" title="Go to paper reference"><i class="bi bi-file-earmark-ppt-fill"></i></a>
    </div>
  </div>
</div>
{% endfor %}
  </div>
</div>
