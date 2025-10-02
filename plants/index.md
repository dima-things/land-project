---
layout: page
title: Plants
---

# Plants

Plant ideas, sorted alphabetically.

{% assign items = site.plants | sort: "title" | reverse %}
<ul>
{% for p in items %}
<li><a href="{{ p.url | relative_url }}">{{ p.title }}</a></li>
{% endfor %}
</ul>
