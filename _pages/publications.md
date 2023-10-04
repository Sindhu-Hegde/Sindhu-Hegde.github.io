---
layout: page
permalink: /publications/
title: Publications
description: Publications in reversed chronological order. A more updated list can be found at <a href='https://scholar.google.com/citations?hl=en&user=cD8J2-kAAAAJ&view_op=list_works&sortby=pubdate'>Google Scholar</a> 
years: [2023, 2022, 2021, 2019, 2018, 2017]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
