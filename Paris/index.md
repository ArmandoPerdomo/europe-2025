---
title: Paris
has_children: true
nav_order: 5
permalink: /paris/
has_toc: true
---

# París

Itinerario detallado para la estancia en París.

## Días

{% assign sorted_pages = site.pages | where_exp:"page", "page.path contains 'Paris'" | where_exp:"page", "page.name contains '.md'" | where_exp:"page", "page.name != 'index.md'" | sort: "name" %}
{% for page in sorted_pages %}
* [{{ page.name | replace: ".md", "" | replace: "_", " " | replace: "-", " " }}]({{ page.url | relative_url }})
{% endfor %}

