---
layout: page
title: Plants
---

{% assign items = site.plants | sort: 'date' | reverse %}
{% for item in items %}
- [{{ item.title }}]({{ item.url | relative_url }}) — {{ item.date | date: "%Y-%m-%d" }}
{% endfor %}
