---
layout: page
permalink: /publications/
title: publications
description:
years: [2022,2021]
nav: false
---


<div class="publications">

Most of the papers available from this list appear in print, and the corresponding copyright is held by the publisher. While the papers can be used for personal use, redistribution or reprinting for commercial purposes is prohibited. Preproceedings versions are available upon request.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f publications -q @*[year={{y}}]* %}
{% endfor %}

</div>
