---
layout: page
title: Shelter
---

{% assign items = site.shelter | sort: 'date' | reverse %}
{% for item in items %}
- [{{ item.title }}]({{ item.url | relative_url }}) — {{ item.date | date: "%Y-%m-%d" }}
{% endfor %}
