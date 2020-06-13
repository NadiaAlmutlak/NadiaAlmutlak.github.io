---
layout: page
permalink: /publications/
title: Research & Presentations
description: 
years: [2020, 2019, 2016]
year: [2020, 2019, 2017, 2016]
---

# Research

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

# Presentations

{% for y in page.year %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f conf -q @*[year={{y}}]* %}
{% endfor %}