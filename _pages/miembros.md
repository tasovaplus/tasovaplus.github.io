---
title: Miembros
permalink: "/miembros/"
author_profile: true
sitemap: false
classes: wide
#layout: collection
#entries_layout: grid
#collection: groups_members
#sort_by: number
---
{% assign universities = site.groups_members | sort: "number" %}

<p float="left">
{% for member in universities %}
<div class="container m-2">
  <div class="d-flex flex-wrap">
  <div class="card">
    <div class="row g-0">
        <div class="col-md-2">
        <a href="{{member.university.url}}" title="Go to URL" target="_blank"><img src="{{member.university.logo}}" class="card-img" alt="{{{member.university.name}}"></a>
        </div>
    <div class="col-md-8">
        <div class="card-body">
        <h6 class="card-title">{{member.university.name}}</h6>
        <p class="card-text" style="font-size: 0.6rem;"><em>IP: {{member.university.ip}}</em></p>
        </div>
    </div>
  </div>
  </div>
  </div>
</div>

<!--
<a href="{{member.university.url}}" target="_blank" title="{{member.university.name}}"><img src="{{member.university.logo}}" alt="{{member.university.name}}" width="200px"/></a>
-->
{% endfor %}
</p>
