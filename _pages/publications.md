---
layout: page
permalink: /publications/
title: Publications
number: 2
description: Publications in reverse chronological order.
years: [2022, 2020, 2017]
nav: true
---
<!-- _pages/publications.md --> 
<div class="publications">

{%- for y in page.years %}

  <h2 class="year">{{y}}</h2>

  {% bibliography -f papers -q @*[year={{y}}]* %}
  
{% endfor %}

</div>
