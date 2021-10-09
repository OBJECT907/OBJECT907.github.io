---
layout: page
permalink: /publications/
title: Publications
description: Publications of 907.
years: [1950,1956,1974]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
