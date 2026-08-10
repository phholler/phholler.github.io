# philipholler — academic website

Personal academic website of **Philip Holler**, doctoral candidate at the
University of Mannheim and researcher at the Mannheim Institute for
Sustainable Energy Studies (MISES).

**Live site:** https://phholler.github.io/

Built with [Hugo](https://gohugo.io/) and the
[HugoBlox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv)
template.

## Deployment

Every push to `main` triggers the **“Deploy website to GitHub Pages”** workflow,
which builds the site with Hugo and publishes it to GitHub Pages. The workflow
can also be run manually from the Actions tab. If a build fails, the previously
published site stays online.

## Local development

```bash
pnpm install
hugo server   # http://localhost:1313
```

## Licensing and credits

- **Site code / theme:** MIT — HugoBlox Academic CV, © Lore Labs (see `LICENSE.md`).
- **Fonts:** Lora, Source Serif 4 and Source Code Pro (SIL Open Font License),
  self-hosted from `assets/dist/font/` so that no visitor data is sent to
  third-party font servers.
- **Thumbnail images:** public domain / CC0, sourced via
  [Openverse](https://openverse.org/).
- **Papers:** the PDFs under `static/uploads/pubs/` are the authors' own
  articles, redistributed under their open-access licences (CC BY); copyright
  remains with the authors and the respective publishers.
- **Site text, CV and photographs:** © Philip Holler. All rights reserved.
