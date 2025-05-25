---
title: Split
has_children: true
nav_order: 6
permalink: /split/
has_toc: true
---

# Split

Itinerario detallado para la estancia en Split.

## Días

{% assign sorted_pages = site.pages | where_exp:"page", "page.path contains 'Split'" | where_exp:"page", "page.name contains '.md'" | where_exp:"page", "page.name != 'index.md'" | sort: "name" %}
{% for page in sorted_pages %}
* [{{ page.name | replace: ".md", "" | replace: "_", " " | replace: "-", " " }}]({{ page.url | relative_url }})
{% endfor %}

