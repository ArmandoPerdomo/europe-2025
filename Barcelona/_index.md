---
title: Barcelona
has_children: true
nav_order: 2
---

# Barcelona

Itinerario detallado para la estancia en Barcelona.

## Días

{% assign sorted_pages = site.pages | where_exp:"page", "page.path contains 'Barcelona'" | where_exp:"page", "page.name contains '.md'" | where_exp:"page", "page.name != '_index.md'" | sort: "name" %}
{% for page in sorted_pages %}
* [{{ page.name | replace: ".md", "" | replace: "_", " " | replace: "-", " " }}]({{ page.url | relative_url }})
{% endfor %}
