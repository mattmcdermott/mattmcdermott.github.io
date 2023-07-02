---
layout: page
permalink: /publications/
title: publications
description: listed in reversed chronological order, grouped by year. See my Google Scholar page for the most up-to-date list.
years: [2023, 2022, 2021, 2020, 2018]
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
