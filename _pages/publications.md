---
layout: page
permalink: /publications/
title: publications
description: Here are some of the fun papers I am working on with my collaborators
years: [2021, 2020, 2018, 2016]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
