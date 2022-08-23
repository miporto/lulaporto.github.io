---
layout: page
permalink: /publications/
title: Publications
number: 2
description: Publications in chronological order.
years: [2017, 2020, 2022]
nav: true
---
<!-- _pages/publications.md --> 
<div class="publications">

{%- for y in page.years %}

  <h2 class="year">{{y}}</h2>

  {% bibliography -f papers -q @*[year={{y}}]* %}
  
{% endfor %}

</div>
