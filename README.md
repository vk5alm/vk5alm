# Lower Murray Radio Club (VK5ALM) — Quarto site

Static rebuild of the club website that was running on GetSimple at
<http://vk5alm.duckdns.org>.

The paid `vk5alm.org` domain is no longer required. Publish this repo to
**GitHub Pages** and the club site will be at:

`https://YOURUSER.github.io/vk5alm/`

## What was converted

| Original GetSimple page | Quarto file |
|---|---|
| Home | `index.qmd` |
| News | `news.qmd` + `news/` |
| Projects | `projects.qmd` + `projects/` |
| Events | `events.qmd` |
| History | `history.qmd` |
| Ham News | `ham-news.qmd` |

Images, the 1923 newspaper PDF, Splat coverage maps, the dual-band antenna sheet,
the MD380 codeplug and the VK5RMB Google Earth zip are in `images/` and `files/`.

A few old CMS plugins (live TEC injector) and extra PDFs were replaced with
public links rather than copied in full.

## Publish on GitHub Pages

```bash
# once Quarto is installed: https://quarto.org/docs/get-started/
cd vk5alm-quarto
quarto publish gh-pages
```

Or render locally and push the `docs/` folder:

```bash
quarto render
```

Then in the GitHub repo: Settings → Pages → Deploy from branch `main` / `/docs`.

## Local preview

```bash
quarto preview
```
