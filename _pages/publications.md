---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
---

{% include bib_search.liquid %}

## Journal articles

<div class="publications">
{% bibliography --query @article %}
</div>

## Book chapters

<div class="publications">
{% bibliography --query @incollection %}
</div>

## Preprints

<div class="publications">
{% bibliography --query @misc %}
</div>
