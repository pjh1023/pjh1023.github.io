---
layout: page
permalink: /publications/
title: Publications
description: 
categories: [Graph Neural Networks]
nav: true
nav_order: 1
sort_field: date
sort_reverse: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.categories %}
  <h4 class="category">{{y}}</h4>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[category={{y}}]* %}
{% endfor %}

</div>
