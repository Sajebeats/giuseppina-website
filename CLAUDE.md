# Giuseppina Mezzelani – LR LIFETAKT Website

## Projektübersicht
Persönliche Beraterinnen-Website für Giuseppina Mezzelani, LR LIFETAKT Partnerin.
Live unter: https://giuseppina-m.de
GitHub Repo: https://github.com/Sajebeats/giuseppina-website
Hosting: GitHub Pages (Branch: main)
Kontakt: josy@giuseppina-m.de | WhatsApp: +4915231717671

---

## Ordnerstruktur

```
giuseppina-website/          ← EINZIGER Arbeitsordner
├── index.html               ← Die gesamte Website (HTML + CSS + JS)
├── CNAME                    ← Domain: giuseppina-m.de
├── impressum.html           ← Standalone Impressum (Fallback)
├── datenschutz.html         ← Standalone Datenschutz (Fallback)
├── images/
│   ├── hero.jpg             ← Hero Portrait (optimiert, 161KB)
│   ├── about.jpg            ← Über-mich Portrait (138KB)
│   ├── work.jpg             ← Laptop-Bild (140KB)
│   ├── cta.jpg              ← Kontakt/CTA Lifestyle (255KB)
│   └── original/            ← Originale PNGs (nicht in Git)
├── pdfs/                    ← LR Kataloge (nicht in Git, zu groß)
├── docs/                    ← Konzept-Dokumente (nicht in Git)
└── .claude/launch.json      ← Vorschau-Server (Port 3456)
```

---

## Design System

### Farben
- --g1: #C9896A  (Terracotta Haupt)
- --g2: #B8705A  (Terracotta Dunkel)
- --gp: #F2DDD2  (Pfirsich Hell)
- --cream: #FDFAF7
- --sand: #F5EDE3
- --dark: #1E1A17

### Schriften
- Headlines: Cormorant Garamond (weight 300/400/500)
- Body: DM Sans (weight 300/400/500)

### Wichtige CSS-Klassen
- .fi = Fade-In Element (per JS animiert)
- .sec = Standard Sektion (padding: 88px 24px)
- .sec-bg = Sand-Hintergrund
- .container = max-width: 1100px
- .lpage = Overlay-Seite (Impressum, Datenschutz, Artikelsuche)
- .pcard = Premium Card mit Hover-Effekt

---

## Deployment
  git add .
  git commit -m "Beschreibung"
  git push origin main
GitHub Pages baut automatisch. Live in ~2 Minuten.

---

## Wichtige Features
1. Artikelsuche – Kunden können LR Artikelnummern nachschlagen (Footer)
2. Quiz – Produktempfehlungs-Quiz (7 Schritte)
3. Impressum/Datenschutz – Als Overlay eingebettet (lpage)
4. WhatsApp CTA – Überall verlinkt (+4915231717671)

---

## Regeln
- IMMER mobile-first testen (375px)
- Bilder IMMER komprimieren vor Git (sips -Z 1200, JPEG 85%)
- Keine externen Libraries – alles vanilla HTML/CSS/JS
- Impressum/Datenschutz NICHT auslagern (GitHub Pages Cache-Probleme)
