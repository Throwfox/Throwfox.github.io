---
layout: page
permalink: /publications/
title: Publications
description: All publications are ordered by year.
years: [2023,2022,2021]
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

<header class="post-header">
  <h1 class="post-title">Manuscript</h1>
  <p class="post-description">The following manuscripts are submitted to the conference or journal and under review.</p>
</header>

<div class="publications">

{%- for y in page.years %}
  {% bibliography -f manuscript -q @*[year={{y}}]* %}
{% endfor %}

</div>
