---
layout: page
title: industry
permalink: /industry/
description: Neurotechnology research and data science with companies.
nav: true
nav_order: 2
horizontal: false
---

<style>
  /* Match the card titles to the page heading: same family, same light weight. */
  .projects .card-title {
    font-weight: 300;
    font-size: 1.6rem;
    line-height: 1.25;
  }
</style>

<!-- pages/projects.md -->
<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
