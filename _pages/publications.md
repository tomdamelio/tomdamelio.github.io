---
layout: page
permalink: /research/
title: research
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<style>
  /* The layout always emits a description paragraph; collapse it when empty
     so the Scholar line sits right under the heading. */
  .post-header .post-description:empty {
    display: none;
  }
  .post-header {
    margin-bottom: 0.5rem;
  }
  .post > article > p:first-of-type {
    margin-top: 0;
  }
</style>

See also my [Google Scholar profile](https://scholar.google.com/citations?user=gldnmWMAAAAJ).

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
