---
layout: about
title: About
permalink: /
subtitle: Assistant Professor at Wrocław University of Science and Technology.
selected_papers: false
social: false
announcements:
  enabled: false
latest_posts:
  enabled: false
---

<div class="row" style="align-items: center; margin-bottom: 1.5rem;">
<div class="col-md-8" markdown="1">

I am a mathematician in the Faculty of Pure and Applied Mathematics at Wrocław University of Science and Technology.
My research concerns stochastic processes, anomalous diffusion, long memory, and statistical inference,
with applications to the analysis of single-particle trajectories.

<nav aria-label="Academic profiles" style="display: flex; flex-wrap: wrap; gap: 0.5rem 1.25rem; align-items: center; margin-bottom: 1.5rem;">
  <span>Profiles:</span>
  <a href="https://orcid.org/{{ site.data.socials.orcid_id }}"><i class="ai ai-orcid" aria-hidden="true"></i> ORCID</a>
  <a href="https://scholar.google.com/citations?user={{ site.data.socials.scholar_userid }}&amp;hl=en"><i class="ai ai-google-scholar" aria-hidden="true"></i> Google Scholar</a>
  <a href="https://www.scopus.com/authid/detail.uri?authorId={{ site.data.socials.scopus_id }}"><i class="ai ai-scopus" aria-hidden="true"></i> Scopus</a>
  <a href="https://github.com/{{ site.data.socials.github_username }}"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
</nav>

<nav aria-label="Explore my work" style="display: flex; flex-wrap: wrap; gap: 0.5rem 1.25rem; align-items: center; margin-bottom: 1.5rem;">
  <a href="{{ '/research/' | relative_url }}">Research →</a>
  <a href="{{ '/publications/' | relative_url }}">Publications →</a>
  <a href="{{ '/students/' | relative_url }}">For students →</a>
  <a href="{{ '/teaching/' | relative_url }}">Teaching →</a>
  <a href="{{ '/cv/' | relative_url }}"><i class="ai ai-cv" aria-hidden="true"></i> CV →</a>
</nav>

</div>
<div class="col-md-4">
  <div style="max-width: 260px; margin: 0 auto;">
    {% include figure.liquid path="assets/img/michal-balcerek.jpg" alt="Michał Balcerek" class="img-fluid rounded" loading="eager" width="3072" height="4080" sizes="(min-width: 768px) 260px, (max-width: 300px) 90vw, 260px" cache_bust=true %}
  </div>
</div>
</div>

## Research interests

<div class="row research-cards">
  <div class="col-md-4 mb-4">
    <div class="card h-100" style="border-radius: 0.75rem;">
      <div class="card-body">
        <h3 class="card-title" style="font-size: 1.1rem; line-height: 1.4;">Anomalous diffusion</h3>
        <p class="card-text">Stochastic modelling of diffusion and complex trajectories.</p>
        <a href="{{ '/research/#anomalous-diffusion' | relative_url }}">Read more →</a>
      </div>
    </div>
  </div>
  <div class="col-md-4 mb-4">
    <div class="card h-100" style="border-radius: 0.75rem;">
      <div class="card-body">
        <h3 class="card-title" style="font-size: 1.1rem; line-height: 1.4;">Long-memory processes</h3>
        <p class="card-text">Stochastic processes with dependence across time.</p>
        <a href="{{ '/research/#long-memory-processes' | relative_url }}">Read more →</a>
      </div>
    </div>
  </div>
  <div class="col-md-4 mb-4">
    <div class="card h-100" style="border-radius: 0.75rem;">
      <div class="card-body">
        <h3 class="card-title" style="font-size: 1.1rem; line-height: 1.4;">Statistical inference</h3>
        <p class="card-text">Statistical methods for single-particle trajectories and experimental data.</p>
        <a href="{{ '/research/#statistical-inference' | relative_url }}">Read more →</a>
      </div>
    </div>
  </div>
</div>

<section class="contact-panel" aria-labelledby="contact">
<h2 id="contact">Contact</h2>

<address style="font-style: normal;">
  <strong>Wrocław University of Science and Technology</strong><br>
  Faculty of Pure and Applied Mathematics · Department of Applied Mathematics · Hugo Steinhaus Center<br>
  Wybrzeże Wyspiańskiego 27, 50-370 Wrocław, Poland<br>
  Room A.3.23 · Building C-19<br>
  <i class="fa-solid fa-envelope" aria-hidden="true"></i> E-mail: <a href="mailto:michal.balcerek@pwr.edu.pl">michal.balcerek@pwr.edu.pl</a>
</address>
</section>
