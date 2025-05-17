---
layout: home
title: Viaje por Europa 2025
nav_order: 1
permalink: /
---

# Itinerario Europa 2025

Bienvenido a mi guía detallada para el viaje por Europa en 2025.

## Ciudades incluidas

{% assign sorted_pages = site.html_pages | sort: "nav_order" %}
{% for page in sorted_pages %}
  {% if page.title and page.has_children %}
* [{{ page.title }}]({{ page.url | relative_url }})
  {% endif %}
{% endfor %}

## Sobre esta guía

Esta guía contiene itinerarios detallados, recomendaciones, costos estimados y otra información práctica para cada destino. Navega por las ciudades en el menú lateral para acceder a los detalles de cada día.

### Características:
- 📍 Enlaces a Google Maps para todas las ubicaciones
- 💶 Estimaciones de presupuesto
- 🕒 Horarios optimizados
- 🍽️ Recomendaciones gastronómicas
- 🚶‍♂️ Tiempos de traslado
