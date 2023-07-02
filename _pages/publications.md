---
layout: page
permalink: /publications/
title: publications
description: listed in reversed chronological order, grouped by year. See my <a href="https://scholar.google.com/citations?user=LPWcdo2gdw4C&hl=en">Google Scholar profile</a> for a complete list.
years: [2023, 2022, 2021, 2020, 2019]
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
