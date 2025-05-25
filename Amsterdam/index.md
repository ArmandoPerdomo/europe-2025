---
title: Amsterdam
has_children: true
nav_order: 4
permalink: /amsterdam/
has_toc: true
---

# Ámsterdam

Itinerario detallado para la estancia en Ámsterdam.

## Días

{% assign sorted_pages = site.pages | where_exp:"page", "page.path contains 'Amsterdam'" | where_exp:"page", "page.name contains '.md'" | where_exp:"page", "page.name != 'index.md'" | sort: "name" %}
{% for page in sorted_pages %}
* [{{ page.name | replace: ".md", "" | replace: "_", " " | replace: "-", " " }}]({{ page.url | relative_url }})
{% endfor %}

