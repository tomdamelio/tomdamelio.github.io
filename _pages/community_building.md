---
layout: page
title: community building
permalink: /community_building/
nav: true
nav_order: 5
---

One of my primary goals in recent years has been to create and nurture communities where scientific and technological knowledge about **<span style="color:#FF6666;">human behavior</span>** is central.

To this end, I have focused on developing ecosystems that connect scientists with:

- The **general public**, through NeuroTransmitiendo;
- The **industry**, via NeuroTechX Buenos Aires;
- Other **scientists**, more recently through the Affective Computing community.

I am committed to fostering an environment where human behavior is not just a field of study, but a catalyst for positive change and the advancement of humanity.

<br>

<!-- pages/community_building.md -->
<div class="projects">
  {% assign sorted_items = site.community_building | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for item in sorted_items %}
      {% assign project = item %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
