# Tinghan (Joe) Ye Website

Personal academic website for Tinghan (Joe) Ye, built with Hugo and Wowchemy.

Live site: <https://joeyetinghan.github.io/>

## Local Development

This site is pinned to Hugo `0.97.3` (see [go.mod](./go.mod) and the deploy
workflow in [.github/workflows/hugo.yml](./.github/workflows/hugo.yml)).
It also uses Hugo modules, so Go must be installed for local builds.

To match production as closely as possible, use Hugo `0.97.3`.
Much newer Hugo releases can break this older Wowchemy setup.

This repo includes Windows PowerShell wrappers that download and use the
correct Hugo version automatically on first run:

```bash
.\scripts\server.ps1
```

Build a production bundle with:

```bash
.\scripts\build.ps1
```

You can also forward arbitrary arguments to the pinned Hugo binary with:

```bash
.\scripts\hugo.ps1 version
```

## Content Structure

- `content/authors/admin/`: biography, education, social links, and avatar
- `content/home/`: homepage sections such as biography, publications, working papers, awards, and contact
- `content/publication/`: publication entries and BibTeX citations
- `static/uploads/`: CV, posters, and slide decks

## Deployment

GitHub Actions builds and deploys the site to GitHub Pages on every push to
`main`, using [.github/workflows/hugo.yml](./.github/workflows/hugo.yml). The
base URL is configured in [config/_default/config.yaml](./config/_default/config.yaml)
and overridden to the Pages URL at build time. In the repository settings,
**Settings → Pages → Build and deployment → Source** must be set to
**GitHub Actions**.
