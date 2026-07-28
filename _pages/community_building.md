---
layout: page
title: community
permalink: /community/
description: Building the institutions that let people learn neuroscience — a Latin American nonprofit, a neurotechnology chapter, and a regional conference.
nav: true
nav_order: 3
---

A field grows through the institutions that let people enter it. Much of my work outside research has gone into building those: an organization that teaches neuroscience to a Spanish-speaking public that had few reliable sources, a local chapter connecting researchers with the neurotechnology industry, and a regional conference that gives students somewhere to present.

The through-line is access. Most of what I know I learned from courses, summer schools and communities that someone else took the trouble to organize — and in Latin America that infrastructure often does not exist until somebody builds it.

---

## Neurotransmitiendo

Co-founder and Board member since 2019 · [neurotransmitiendo.org](https://www.neurotransmitiendo.org/)

A Latin American nonprofit dedicated to democratising access to neuroscience and behavioural science for Spanish-speaking communities. It has grown to **over 33,000 followers**, a team of **more than 30 researchers**, and is now one of the largest science education communities in the region.

- Member of the Board of Directors since its founding, with responsibilities in nonprofit governance, strategic planning and organizational development.
- Created and directed a **Diploma Program in Cognitive Neuroscience** — over 300 students, more than 40% on scholarships — with faculty from leading international universities.
- Founded and organized the **first Latin American Conference of Cognitive Neuroscience** (2025), now in its second edition (2026), with over 400 attendees and 100+ posters across both years.
- Host and general producer of the organization's [podcast](https://open.spotify.com/show/4h97z3s1rTwM2gKH8bYd1J), interviewing neuroscientists from across Latin America, alongside educational content on [Instagram](https://www.instagram.com/neurotransmitiendo/).

---

## NeuroTechX Buenos Aires

Co-founder and team leader · [neurotechx.com](https://neurotechx.com/)

A local chapter of the world's largest nonprofit neurotechnology community, with the mission of advancing neurotechnology by integrating artificial intelligence with neuroscience.

- Organized nine seminars on computational neuroscience.
- Ran workshops on AI and neuroscience at national and international conferences.
- Hosted meetups with founders and researchers from the neurotech ecosystem.
- Led the chapter in a two-day hybrid hackathon organized by NeuroTechX global, with 30 in-person participants.
- Grew the community to **over 200 active members** on Slack.

---

## Policy

Invited to join **UNESCO's expert committee** at the Latin American meeting on the ethical challenges of neurotechnologies.

---

<div class="projects">
  {% assign sorted_items = site.community_building | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for item in sorted_items %}
      {% assign project = item %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
