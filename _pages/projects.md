---
layout: page
title: industry
permalink: /industry/
description: Research and data science inside companies building neurotechnology.
nav: true
nav_order: 2
horizontal: false
---

Some of the work I care about most has happened inside companies rather than laboratories. The problem there is the same one that runs through my research, only sharper: a sensor is not an instrument until someone specifies what it should measure, builds the processing that makes the signal usable, and designs the protocol that turns it into evidence.

<!-- pages/projects.md -->
<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
