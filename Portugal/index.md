---
title: Portugal
has_children: true
nav_order: 8
permalink: /portugal/
has_toc: true
---

# Portugal

Itinerario detallado para la estancia en Portugal.

## Días

{% assign sorted_pages = site.pages | where_exp:"page", "page.path contains 'Portugal'" | where_exp:"page", "page.name contains '.md'" | where_exp:"page", "page.name != 'index.md'" | sort: "name" %}
{% for page in sorted_pages %}
* [{{ page.name | replace: ".md", "" | replace: "_", " " | replace: "-", " " }}]({{ page.url | relative_url }})
{% endfor %}

