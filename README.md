# ZERO Freerunning — Open Dag Certificaatgenerator

Persoonlijk A4-liggend certificaat + deelkaart (1080×1920) voor de ZERO Open Dag.

## Bestanden

- `index.html` — formulier, certificaatpreview, QR, deelkaart
- `certificaat.css` — scherm + print (A4 landscape)
- `certificaat-bg.jpg` — frame / medal / swoosh
- `vendor/qrcode.min.js` — lokale QR-lib (offline na laden)

## Gebruik

1. Open `index.html` (of via lokale webserver).
2. Vul naam, datum, max. 3 missies, optioneel coach + boodschap.
3. **Genereer certificaat** → preview.
4. **Download / Print PDF** → A4 liggend, marges Geen, achtergrondgraphics aan.
5. **Download deelkaart** → PNG met alleen voornaam.

## URL-parameters

`?naam=&datum=&coach=&msg=` (of `boodschap=`) `&missies=landing,vault,doorzetter`

Missie-ids: `landing`, `precision`, `vault`, `doorzetter`, `creatief`, `samen`

## Print-tip

Opslaan als PDF · A4 · Liggend · Marges Geen · Achtergrondgraphics aan.
