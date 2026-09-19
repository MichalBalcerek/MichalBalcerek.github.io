# Personal site instructions

This is Michał Balcerek's personal site created from the al-folio v1 starter.

- Repository: `MichalBalcerek/MichalBalcerek.github.io`.
- Production URL: `https://michalbalcerek.github.io/`.
- `_config.yml` must use an empty `baseurl`. Upstream docs sometimes use `/al-folio` for their demo; do not apply that path here.
- Preserve user-authored content. Never invent biographical details, publications, positions, or achievements.
- Customize `_config.yml`, `_data`, `_pages`, collections, and assets first. Keep shared runtime in its pinned gems; read `docs/BOUNDARIES.md` before adding runtime overrides.
- Keep Gemfile dependencies and `_config.yml` plugin activation consistent.
- Commit source changes to `main`; the deployment workflow generates `gh-pages`.
- Use `npm run lint:prettier`, `npm run lint:style-contract`, `bundle exec al-folio upgrade audit --no-fail`, and `JEKYLL_ENV=production bundle exec jekyll build` to validate.
- If local gem-owned overrides are introduced, run `bundle exec al-folio upgrade overrides audit` and track the approved override manifest.
