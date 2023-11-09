---
layout: page
permalink: /publications/graph
title: Publications
description: <sup>*</sup>authors contributed equally. <br> <br>
  <a href=uncertainty>#Uncertainty Quantification</a>
  <a href=latent>#Latent Variable Models</a>
  <a href=dynamical>#Dynamical Systems</a>
  <a href=graph style="color:var(--global-theme-color)">#Graph Learning</a>
  <a href=sensor>#Sensors</a>
years: [2021, 2020, 2019]
nav: false
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}, graph=true]*%}
{% endfor %}

</div>
