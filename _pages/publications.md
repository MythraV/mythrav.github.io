---
layout: page
permalink: /publications/
title: Publications
description: Publications in reverse chronological order
years: [2023, 2022, 2021, 2019, 2018, 2015]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
