---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  <img src="/assets/img/git_rate.gif" alt="project thumbnail">
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
