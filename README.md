# raum-planer-online.de — SEO Landing Pages

## Dateistruktur

```
project-root/
├── index.html                                ← Komplette HTML-Seite (Header + 10 Blöcke + Footer)
├── css/
│   ├── global.css                            ← Gemeinsame Styles (Reset, Typo, Header, Footer, Buttons)
│   └── 3d-raumplaner-online-kostenlos.css    ← Seitenspezifische Styles
└── README.md                                 ← Diese Datei
```

## Design-System

- **Fonts:** Playfair Display (Überschriften, Gewicht 400/600) + DM Sans (Fließtext, Gewicht 400–700)
- **Farben:**
  - Hintergrund: `#faf9f7` (warmes Off-White)
  - Text: `#1a1a2e` (dunkles Anthrazit)
  - Akzent: `#2d5a27` (erdiges Grün)
- **Icons:** Ausschließlich Custom-SVGs (Stroke-basiert, 1.2–1.5px, currentColor)
- **Responsive:** Mobile-First, Breakpoint bei 768px
- **Kein JavaScript** im Browser — reine HTML/CSS-Lösung
- **Maximale Seitengewicht:** ~50KB (ohne Google Fonts CDN)

## Neue Landingpage hinzufügen

1. **index.html kopieren** und `<head>` Meta-Tags anpassen (Title, Description, Canonical, OG, JSON-LD)
2. **Seitenspezifisches CSS erstellen:** `css/{neuer-slug}.css`
3. **Inhaltsblöcke** im `<main>` anpassen
4. **Header und Footer** bleiben identisch — sie sind direkt in der HTML-Datei eingebettet

## SEO-Checkliste

- [x] Title-Tag: unter 60 Zeichen, enthält Hauptkeyword + Jahr
- [x] Meta-Description: 150–160 Zeichen mit Keyword
- [x] Einzelnes H1 mit Hauptkeyword
- [x] Logische Heading-Hierarchie (H1 → H2 → H3)
- [x] Open-Graph-Tags komplett
- [x] JSON-LD Schemas: Article, WebApplication, ItemList, FAQPage
- [x] FAQ-Accordion mit `<details>/<summary>` (funktioniert ohne JS)
- [x] Responsive Tabellen (horizontal scrollbar auf Mobilgeräten)
- [x] Semantisches HTML5 durchgehend
- [x] Alle CTAs verlinken auf https://raum-planer-online.de
