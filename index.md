---
layout: page
title: Home
---

## Sections
- [Plants]({{ 'plants/' | relative_url }})
- [Land]({{ 'land/' | relative_url }})
- [Shelter]({{ 'shelter/' | relative_url }})

## Latest posts
{% assign items = site.plants | concat: site.land | concat: site.shelter | sort: 'date' | reverse %}
{% for item in items limit:10 %}
- [{{ item.title }}]({{ item.url | relative_url }}) — {{ item.date | date: "%Y-%m-%d" }}
{% endfor %}
