---
layout: page
title: Teaching
permalink: /teaching/
nav: true
nav_order: 4
toc:
  sidebar: right
---

Course information and teaching materials will be collected here. Select a course below to visit its page.

## Office hours

<div class="card mb-4">
  <div class="card-body">
    <p class="card-text mb-0">Office hours and contact details will be announced here.</p>
  </div>
</div>

## Courses

The course pages below are being prepared. Schedules, materials, and assessment information will be added to each page.

<div class="row">
  {% assign courses = site.teachings | sort: "importance" %}
  {% for course in courses %}
  <div class="col-md-6 mb-4">
    <div class="card h-100" style="border-radius: 0.75rem;">
      <div class="card-body" style="display: flex; gap: 1rem; align-items: flex-start;">
        <span aria-hidden="true" style="font-size: 1.5rem; color: var(--global-theme-color);">{{ course.symbol }}</span>
        <div>
          <h3 class="card-title" style="font-size: 1.1rem; line-height: 1.4; margin: 0 0 0.5rem;"><a href="{{ course.url | relative_url }}">{{ course.title }}</a></h3>
          <p class="card-text mb-0">{{ course.description }}</p>
        </div>
      </div>
    </div>
  </div>
  {% endfor %}
</div>

## Other materials

Additional teaching resources will be added here.
