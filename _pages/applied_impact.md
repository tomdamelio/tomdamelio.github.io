---
layout: page
title: applied impact
permalink: /applied_impact/
description: Bringing behavioral science and neurotechnology to industry and public policy.
nav: true
nav_order: 4
---

<!-- pages/applied_impact.md -->
<div class="projects">
  {% assign sorted_items = site.applied_impact | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for item in sorted_items %}
      {% assign project = item %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
