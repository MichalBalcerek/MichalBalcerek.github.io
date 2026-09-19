---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 1
---

{% include bib_search.liquid %}

## Journal articles

<div class="publications">
{% bibliography --query @article %}
</div>

## Preprints

<div class="publications">
{% bibliography --query @misc %}
</div>
