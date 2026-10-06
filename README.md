# Personal website

[![Deploy](https://github.com/estefafdez/estefafdez.github.io/actions/workflows/deploy.yml/badge.svg)](https://github.com/estefafdez/estefafdez.github.io/actions/workflows/deploy.yml)

Jekyll CV and portfolio at [estefafdez.com](https://estefafdez.com/).
The QA blog is a separate site at [unaqaenapuros.com](https://unaqaenapuros.com/).

## Run locally

Install Ruby and Bundler, then:

```bash
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000. Run `bundle exec jekyll build` for a static build.

## Structure

- `_config.yml`: site configuration and the version-2 CV sections.
- `_data/`: supporting CV content.
- `assets/main.scss`: styling.
- `images/`: profile image and favicon.
- `cv_markdown/`: downloadable CV sources and PDF.
- `CNAME`: custom domain.

The theme is configured in `_config.yml`; keep the existing theme and author
credits when editing content.

## Deployment

`.github/workflows/deploy.yml` builds and deploys GitHub Pages on pushes to
`master`, or via its manual Run workflow button. Pull requests do not deploy the
site. GitHub Pages must use GitHub Actions as its deployment source.
Keep `CNAME` and the configured `url` aligned with the custom domain.

See [CONTRIBUTING.md](CONTRIBUTING.md) and [SECURITY.md](SECURITY.md).
