# Publish on GitHub Pages

The site is configured for the repository `MichalBalcerek/MichalBalcerek.github.io` and the address `https://michalbalcerek.github.io/`.

1. Sign in to GitHub as **MichalBalcerek** and check whether a repository named **MichalBalcerek.github.io** already exists. Do not overwrite an existing site. A public unauthenticated check returned 404 during preparation, which cannot rule out a private repository.
2. If it does not exist, create a **public** repository with that name. Upload or push the contents of this folder to its `main` branch, keeping the directories intact and including `.github/workflows/deploy.yml`. Do not upload `_site`, `node_modules`, or local caches.
3. In **Settings → Actions → General → Workflow permissions**, choose **Read and write permissions** if the deployment needs them. The supplied workflow declares `contents: write` to publish the generated site.
4. Open **Actions → Deploy site** and wait for the build to succeed. If needed, use **Run workflow**. This creates the `gh-pages` branch.
5. In **Settings → Pages**, choose **Deploy from a branch**, select **gh-pages**, choose **/(root)**, and save.
6. Wait for Pages deployment, then visit **https://michalbalcerek.github.io/**.

Keep `_config.yml` set to:

```yaml
url: https://michalbalcerek.github.io
baseurl: ""
```

## Local preview

With Ruby, Bundler, Node.js/npm, and ImageMagick installed:

```sh
bundle install
npm ci
bundle exec jekyll serve
```

Then open `http://localhost:4000/`. This personal website uses the domain root; do not add the upstream demo's `/al-folio` base path.

Python and nbconvert are only needed locally if you later add Jupyter notebook content. The deployment workflow installs them automatically.

## Validation

```sh
npm run lint:prettier
npm run lint:style-contract
bundle exec al-folio upgrade audit --no-fail
JEKYLL_ENV=production bundle exec jekyll build
```

Official reference: [al-folio installation and deployment](https://github.com/alshedivat/al-folio/blob/main/docs/INSTALL.md).
