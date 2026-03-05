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

## Rechtlicher Hinweis

Impressum/Datenschutz sind als Muster angelegt und müssen auf den realen Einzelfall angepasst werden.
