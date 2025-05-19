---
title: Roma
has_children: true
nav_order: 9
permalink: /roma/
---

# Roma

Itinerario detallado para la estancia en Roma.

## Días

{% assign sorted_pages = site.pages | where_exp:"page", "page.path contains 'Roma'" | where_exp:"page", "page.name contains '.md'" | where_exp:"page", "page.name != 'index.md'" | sort: "name" %}
{% for page in sorted_pages %}
* [{{ page.name | replace: ".md", "" | replace: "_", " " | replace: "-", " " }}]({{ page.url | relative_url }})
{% endfor %}
