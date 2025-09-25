---
layout: page
title: Plants
---

# Plants

Intro text here.

{% assign items = site.plants | sort: "date" | reverse %}
<ul>
{% for p in items %}
  <li><a href="{{ p.url }}">{{ p.title }}</a></li>
{% endfor %}
</ul>
