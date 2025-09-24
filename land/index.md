---
layout: page
title: Land
---

{% assign items = site.land | sort: 'date' | reverse %}
{% for item in items %}
- [{{ item.title }}]({{ item.url | relative_url }}) — {{ item.date | date: "%Y-%m-%d" }}
{% endfor %}
