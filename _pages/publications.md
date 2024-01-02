---
layout: page
title: Publications
permalink: /publications/
description: Publications in reversed chronological order. My <a href="https://scholar.google.com/citations?user=tQTAiXwAAAAJ&hl=en"> Google Scholar </a> is more likely to be up to date.
years: [2024, 2023, 2022, 2021, 2020]
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