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
  <a href="{{member.university.url}}" title="{{member.university.name}}"><img src="{{member.university.logo}}" alt="{{member.university.name}}" width="200px"/></a>
{% endfor %}
</p>
