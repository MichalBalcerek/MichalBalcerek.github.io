---
layout: page
title: Teaching
permalink: /teaching/
nav: true
nav_order: 4
toc:
  sidebar: right
---

My teaching schedule and course pages are collected here.

## Schedule

**Winter semester 2026/27** · 1 October 2026–3 February 2027

Regular teaching slots are listed below. All times are local to Wrocław (Europe/Warsaw).
For individual teaching dates, breaks, and changes, please check the [current timetable in USOS][usos-timetable].

{% assign analysis_url = '/teaching/analiza-matematyczna-1/' | relative_url %}
{% assign insurance_url = '/teaching/non-life-insurance-mathematics/' | relative_url %}
{% assign numerical_url = '/teaching/metody-numeryczne/' | relative_url %}

### Tuesday

<div role="region" aria-label="Tuesday teaching schedule" tabindex="0" style="overflow-x: auto;" markdown="1">

| Time        | Course and group                                                                                        | Building · room |
| ----------- | ------------------------------------------------------------------------------------------------------- | --------------- |
| 07:30–09:00 | [Analiza matematyczna 1]({{ analysis_url }})<br><small>Lecture · group 1 · 13IEA0-25S101O00111W</small> | C-1 · 201/203   |
| 09:15–11:00 | [Non-life insurance mathematics]({{ insurance_url }})<br><small>Laboratory · group 2</small>            | C-19 · A.0.5    |
| 13:15–15:00 | [Non-life insurance mathematics]({{ insurance_url }})<br><small>Project · group 1</small>               | L-1 · 116       |

</div>

### Wednesday

<div role="region" aria-label="Wednesday teaching schedule" tabindex="0" style="overflow-x: auto;" markdown="1">

| Time        | Course and group                                                                             | Building · room |
| ----------- | -------------------------------------------------------------------------------------------- | --------------- |
| 07:30–09:00 | [Non-life insurance mathematics]({{ insurance_url }})<br><small>Laboratory · group 1</small> | C-19 · A.0.5    |
| 09:15–11:00 | [Metody numeryczne]({{ numerical_url }})<br><small>Laboratory · group 4</small>              | C-19 · A.0.6    |

</div>

### Friday

<div role="region" aria-label="Friday teaching schedule" tabindex="0" style="overflow-x: auto;" markdown="1">

| Time        | Course and group                                                                                          | Building · room |
| ----------- | --------------------------------------------------------------------------------------------------------- | --------------- |
| 07:30–09:00 | [Analiza matematyczna 1]({{ analysis_url }})<br><small>Exercises · group 2 · 13IEA0-25S101O00111C</small> | C-4 · 31        |
| 11:15–13:00 | [Analiza matematyczna 1]({{ analysis_url }})<br><small>Exercises · group 2 · 13EBR0-25S101O00111C</small> | D-1 · 28        |
| 13:15–15:00 | [Analiza matematyczna 1]({{ analysis_url }})<br><small>Exercises · group 1 · 13IEA0-25S101O00111C</small> | C-2 · 304       |

</div>

<p class="text-muted"><small>Schedule checked on 20 September 2026. The USOS course codes distinguish the Analiza matematyczna 1 groups.</small></p>

[usos-timetable]: https://web.usos.pwr.edu.pl/kontroler.php?_action=katalog2/osoby/pokazPlanZajecStudenta&plan_division=semester&plan_timebase_sel_timebase=1790805600&token=S7QysqoutjKzUspPykpNLlGyTrQyBImYAkWK4zNTlKwzrYwtLA2MrWuLrcytlFIrCjKLUotBwobmloaGBgamFobWtQA%3D08ea26162cc6c42552c89571a01f972a553d464e

## Office hours

<div class="card mb-4">
  <div class="card-body">
    <p class="card-text mb-0">Office hours and contact details will be announced here.</p>
  </div>
</div>

## Courses

The course pages below are being prepared. Materials and assessment information will be added to each page.

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
