# ZERO Freerunning — Certificaatgenerator

Statische generator voor persoonlijke ZERO Freerunning-certificaten + Instagram/WhatsApp deelkaart.

## Bestanden

- `index.html` — generator + certificaat
- `certificaat.css` — layout, print (A4 landscape), mobiel
- `certificaat-bg.jpg` — achtergrondontwerp

Geen build-stap. Werkt op GitHub Pages.

## Lokaal openen

Open `index.html` via een lokale server (niet als `file://` als fonts/assets blokkeren), bijvoorbeeld:

```bash
python3 -m http.server 8080
```

Ga naar `http://localhost:8080`.

## GitHub Pages

1. Push deze map naar een public repo (root of `/docs`).
2. Settings → Pages → Deploy from branch `main` / root.
3. Live URL: `https://<user>.github.io/<repo>/`

## URL-parameters

| Param | Voorbeeld | Betekenis |
|-------|-----------|-----------|
| `naam` | `Emma%20de%20Vries` | Deelnemer |
| `datum` | `2026-08-12` | Datum (ISO) |
| `coach` | `Sam` | Coachnaam (optioneel) |
| `msg` / `boodschap` | `Sterk%20gedaan` | Coachboodschap (max 120) |
| `missies` | `landing,vault,doorzetter` | Max 3 ids |

Missie-ids: `landing`, `precision`, `vault`, `doorzetter`, `creatief`, `samen`

Voorbeeld:

`?naam=Emma%20de%20Vries&datum=2026-08-12&missies=landing,vault&coach=Sam&msg=Sterk%20gedaan`

## Acties in de UI

- **Genereer certificaat**
- **Download / Print PDF** (browser: Opslaan als PDF, A4 liggend, marges Geen)
- **Download deelkaart** (1080×1920 PNG, alleen voornaam)
- **Opnieuw instellen**

## Print-tip

A4 landscape, marges “Geen”, achtergrondgraphics aan.
