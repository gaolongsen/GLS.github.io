---
layout: page
permalink: /publications/
title: publications
description: Selected publications, not full list.
years: [2024, 2023]
nav: true
nav_order: 1
---

A complete list also including  publications can be found

<!-- _pages/publications.md -->

<div class="publications">


{%- for y in page.years %}

  <h2 class="year">{{y}}</h2>

  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
