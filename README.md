# Michał Balcerek — personal website

A personal academic website based on [al-folio](https://github.com/alshedivat/al-folio).

Intended address: **https://michalbalcerek.github.io/**.

## Edit your content

| Content                              | File                                |
| ------------------------------------ | ----------------------------------- |
| Biography                            | `_pages/about.md`                   |
| Publications                         | `_bibliography/papers.bib` (BibTeX) |
| Projects                             | Add Markdown files in `_projects/`  |
| CV                                   | `_data/cv.yml`                      |
| GitHub and other public links        | `_data/socials.yml`                 |
| Name, description, and site settings | `_config.yml`                       |

The initial site contains only the name Michał Balcerek, the description “Mathematician.”, and a GitHub profile link. Publications, projects, and CV details are intentionally empty.

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

## Add CV details

Edit `_data/cv.yml`. Its empty `sections: {}` can be replaced with sections such as Education, Experience, Awards, or Publications. The format is documented in [the al-folio customization guide](https://github.com/alshedivat/al-folio/blob/main/docs/CUSTOMIZE.md#modifying-the-cv-information). No CV PDF is linked until you add one.

## Setup and preview

See [SETUP.md](SETUP.md) for GitHub Pages configuration and local preview instructions.

The original template documentation is retained in `docs/`. The al-folio theme and runtime are loaded through the pinned dependencies in `Gemfile` and `Gemfile.lock`; there are no local runtime overrides.
