---
layout: page
permalink: /publications/
title: Publications
description: Check the full publications <a href="https://scholar.google.com/citations?user=_ad3YG8AAAAJ&hl=en"><b>here</b></a>
years: [2023,2022,2021,2020,2018,2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
