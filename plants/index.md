---
layout: page
title: Plants
---

Plant ideas, sorted alphabetically.

{% assign items = site.plants | sort: "title" %}
{% for item in items %}
- [{{ item.title }}]({{ item.url | relative_url }})
{% endfor %}
