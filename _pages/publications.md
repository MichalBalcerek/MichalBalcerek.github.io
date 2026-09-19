---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 1
---

{% capture publication_count %}{% bibliography_count %}{% endcapture %}
{% assign publication_count = publication_count | plus: 0 %}
{% if publication_count > 0 %}
{% include bib_search.liquid %}

<div class="publications">
{% bibliography %}
</div>
{% else %}
<p>Publications will be added here.</p>
{% endif %}
