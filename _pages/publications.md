---
layout: page
permalink: /publications/
title: publications
description: history of publications and scientific production over the years
years_one: [2022,2020]
years_two: [2023,2022,2021,2019]
years_three: [2022]
nav: true
nav_order: 3
---
<!-- ↓ papers in peer-reviewed journals -->
<h3 class="mt-4">papers in peer-reviewed journals</h3>
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years_one %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


.


.


.


<!-- ↓ presentations in meetings and symposiums -->
<h3 class="mt-4">presentations in meetings and symposiums</h3>
<div class="publications">

{%- for y in page.years_two %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f presentations -q @*[year={{y}}]* %}
{% endfor %}

</div>


.


.


.


<!-- ↓ thesis -->
<h3 class="mt-4">thesis</h3>
<div class="publications">

{%- for y in page.years_three %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f thesis -q @*[year={{y}}]* %}
{% endfor %}

</div>