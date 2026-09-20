# Michał Balcerek — personal website

A personal academic website based on [al-folio](https://github.com/alshedivat/al-folio).

Website: **https://michalbalcerek.github.io/**.

## Edit your content

| Content                               | File                                |
| ------------------------------------- | ----------------------------------- |
| Biography                             | `_pages/about.md`                   |
| Research overview and technical notes | `_pages/research.md`                |
| Thesis topics and student projects    | `_pages/students.md`                |
| Publications                          | `_bibliography/papers.bib` (BibTeX) |
| Projects                              | Add Markdown files in `_projects/`  |
| CV                                    | `_data/cv.yml`                      |
| Teaching overview and office hours    | `_pages/teaching.md`                |
| Individual course pages               | Markdown files in `_teachings/`     |
| GitHub and other public links         | `_data/socials.yml`                 |
| Name, description, and site settings  | `_config.yml`                       |

The navigation is About, Research, Publications, For students, Teaching, and CV. Research links to the project pages, and the existing `/projects/` address remains available. Course pages are starter pages; fill in their schedules, materials, and assessment details when ready.

You can edit these files directly on GitHub. Commit changes to `main`; the **Deploy site** workflow rebuilds the website automatically. Do not edit the generated `gh-pages` branch.

## Add a project

Create `_projects/my-project.md` with this structure, then replace the title, description, and text with your own content:

```markdown
---
layout: page
title: Project title
description: A short description.
importance: 1
---

Your project description goes here.
```

Project cards appear automatically on the Projects page. Add images under `assets/img/` if desired.

## Update research and student pages

Edit `_pages/research.md` for current research topics, mathematical overviews, and links to representative publications. Technical overviews use native `<details>` elements and MathJax; keep `markdown="1"` on the expandable blocks so that paragraphs and equations render correctly. Research projects are listed from the `_projects/` collection.

Edit `_pages/students.md` for proposed thesis topics, supervision information, and theses grouped by academic year. Preserve the distinction between supervised theses and the earlier work supported through consultations. Keep any availability notice explicitly dated; the imported 2025/26 notice does not establish availability for later years.

## Add CV details

Edit the entries and sections in `_data/cv.yml`. The format is documented in [the al-folio customization guide](https://github.com/alshedivat/al-folio/blob/main/docs/CUSTOMIZE.md#modifying-the-cv-information).

## Update teaching pages

Edit `_pages/teaching.md` to update office hours and general teaching information. Each course has its own file in `_teachings/`:

- `metody-numeryczne.md` — Metody numeryczne
- `analiza-matematyczna-1.md` — Analiza matematyczna 1
- `non-life-insurance-mathematics.md` — Non-life insurance mathematics

Replace the placeholder text under the course headings with your content. Upload handouts under `assets/pdf/` and link them with, for example, `[Problem set 1]({{ '/assets/pdf/problem-set-1.pdf' | relative_url }})`.

To add a course, copy an existing course file, give it a unique `permalink` beginning with `/teaching/`, and update its `title`, `description`, and `importance`. The Teaching overview lists course cards automatically in `importance` order. `symbol` controls the decorative symbol on the card, and `nav: false` keeps the course out of the main navigation.

## Setup and preview

See [SETUP.md](SETUP.md) for GitHub Pages configuration and local preview instructions.

The original template documentation is retained in `docs/`. The al-folio theme and runtime are loaded through the pinned dependencies in `Gemfile` and `Gemfile.lock`. The cyan and neon-pink palette lives in `assets/css/main.scss`, which imports the shared theme modules and adds personal styles. This local entry-point override is tracked in `.al-folio-overrides.yml`; review it when upgrading the theme.
