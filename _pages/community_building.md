---
layout: archive
title: "Community Building"
permalink: /community_building/
author_profile: true
---

One of my primary goals in recent years has been to create and nurture communities where scientific and technological knowledge about <span style="color:#FF6666;">**human behavior**</span> is central.

To this end, I have focused on developing ecosystems that connect scientists with:

- The **general public**, through NeuroTransmitiendo;
- The **industry**, via NeuroTechX Buenos Aires;
- Other **scientists**, more recently through the Affective Computing community.

I am committed to fostering an environment where human behavior is not just a field of study, but a catalyst for positive change and the advancement of humanity.


<nbsp>

{% include base_path %}

{% assign ordered_pages = site.community_building | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}