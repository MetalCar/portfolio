# Hugo Portfolio (Dracula Inspired)

Dieses Projekt ist eine pflegeleichte Portfolio-Website mit Hugo.

## Inhalte pflegen

Die wichtigsten Inhalte liegen in:

- `data/profile.yaml` (Name, Rolle, Intro, Skills, Kontakt)
- `data/timeline.yaml` (Lebenslauf-Stationen)
- `content/impressum.md`
- `content/datenschutz.md`

## Lokal starten mit Docker Compose

```bash
docker compose up
```

Danach ist die Website unter `http://localhost:1313` erreichbar.

## Build mit Docker Compose

```bash
docker compose run --rm hugo
```

Der statische Output liegt in `public/`.

## Deployment mit GitHub Pages

Der Workflow liegt in `.github/workflows/deploy-pages.yml` und deployed bei Push auf den Branch `release`.

1. In GitHub unter `Settings > Pages` bei `Source` die Option `GitHub Actions` aktivieren.
2. Neue Änderungen auf `release` pushen:

```bash
git checkout release
git merge main
git push
```

Danach wird die Seite automatisch nach GitHub Pages ausgerollt.

## Rechtlicher Hinweis

Impressum/Datenschutz sind als Muster angelegt und müssen auf den realen Einzelfall angepasst werden.
