---
layout: page
title: community
permalink: /community/
description: Neuroscience education, neurotech community and policy in Latin America.
nav: true
nav_order: 3
---

<style>
  /* Match the card titles to the page heading: same family, same light weight. */
  .projects .card-title {
    font-weight: 300;
    font-size: 1.6rem;
    line-height: 1.25;
  }
</style>

<div class="projects">
  {% assign sorted_items = site.community_building | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for item in sorted_items %}
      {% assign project = item %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
