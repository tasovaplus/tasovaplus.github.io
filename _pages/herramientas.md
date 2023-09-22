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
      {% if tool.authors %}
      <p class="card-text" style="font-size: 0.6rem;"><em>{{tool.authors}}</em></p>
      {% endif %}
      <a href="{{tool.link}}" title="Go to URL"><i class="bi bi-box-arrow-up-right"></i></a>
      {% if tool.doi %}
        <a href="{{tool.doi}}" title="Go to paper reference"><i class="bi bi-file-earmark-ppt-fill"></i></a>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}
  </div>
</div>
