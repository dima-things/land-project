---
layout: home
title: Home
---

## Sections
- [Plants]({{ 'plants/' | relative_url }})
- [Land]({{ 'land/' | relative_url }})
- [Shelter]({{ 'shelter/' | relative_url }})

## Latest updates
{% for post in site.posts limit:10 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
