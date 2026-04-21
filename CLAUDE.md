# CLAUDE.md — Giuseppina Mezzelani Website

Lies diese Datei zu Beginn jeder Session vollständig durch, bevor du arbeitest.

---

## Projekt-Überblick

**Website für:** Giuseppina Mezzelani  
**Domain:** (bei Hostinger — Domain hier eintragen, z.B. giuseppina-mezzelani.de)  
**Zweck:** Persönliche Berater-Website für LR LIFETAKT Produkte  
**Zielgruppe:** Frauen 25–55, gesundheitsbewusst, interessiert an natürlichen Produkten, Wellness und Schönheit  
**Sprache:** Deutsch  

---

## Was Giuseppina macht

LR LIFETAKT Beraterin — sie berät persönlich und kostenlos zu:
- **Aloe Vera** Produkten (Trinken, Körperpflege)
- **Nahrungsergänzung** (Vitamine, Mineralstoffe)
- **Beauty von innen** (Kollagen, Hautpflege)
- **Body Mission** (Abnehmen, Wohlbefinden)

Wichtig: Sie ist **keine Ärztin**, macht **keine Heilversprechen** — alles ist ehrliche, persönliche Empfehlung.  
Kontakt läuft hauptsächlich über **WhatsApp**.

---

## Design-System

### Farben
```
--g1: #C9896A   (Hauptfarbe, warmes Terrakotta)
--g2: #B8705A   (Dunkleres Terrakotta, Links & Akzente)
--g3: #9A5A44   (Tiefes Terrakotta)
--gp: #F2DDD2   (Helles Rosa, Badges & Highlights)
--gm: #E8C4B0   (Mittleres Rosa, Borders)
--gl: #F5EDE3   (Sehr helles Sand, Backgrounds)
--cream: #FDFAF7 (Seiten-Hintergrund)
--dark: #2C2C2C  (Texte)
```

### Schriften
- **Headlines:** Cormorant Garamond (serif, elegant, leicht)
- **Body/UI:** DM Sans (sans-serif, modern, lesbar)

### Design-Prinzipien
- Feminin, warm, hochwertig — wie ein Premium Beauty-Brand
- Viel Weißraum, sanfte Schatten, abgerundete Ecken (14px)
- Animationen: subtil, `transition: all .28s`
- Mobile-first — alle Breakpoints bei max-width: 768px

---

## Datei-Struktur

```
giuseppina-website/
├── index.html          ← Haupt-HTML (alles in einer Datei — kein Framework)
├── images/             ← Alle Fotos (JPG/PNG)
├── pdfs/               ← LR Produktkatalog PDFs
├── CLAUDE.md           ← Diese Datei
└── .gitignore
```

### Warum alles in index.html?
Einfachstes Deployment: eine Datei ändern, pushen, live. Kein Build-Prozess, kein Node.js, keine Abhängigkeiten.

---

## Sections auf der Website

1. **Header/Nav** — fixiert, mit Logo, Navigation, WhatsApp-Button
2. **Hero** — großes Bild, Headline, Trust-Zahlen
3. **Trust-Band** — dunkler Streifen mit 4 Vertrauens-Punkten
4. **Über mich** — persönliches Foto + Text + Qualifikationen
5. **Produkte** — Tabs: Aloe Vera / Nahrungsergänzung / Beauty / Body Mission
6. **Quiz** — Bedarfs-Quiz für persönliche Empfehlungen  
7. **Beratung buchen** — WhatsApp + Kalender CTA
8. **Bewertungen** — Kundenstimmen
9. **FAQ** — häufige Fragen
10. **Footer** — Links, Impressum, Datenschutz

---

## Regeln für Änderungen

1. **Kein Framework einführen** — bleibt als statisches HTML/CSS/JS
2. **Keine externen Dependencies** hinzufügen außer Google Fonts (bereits eingebunden)
3. **CSS-Variablen** immer aus `:root` nutzen, keine Hardcoded-Farben
4. **Responsive:** jede Änderung auch für mobile (768px) testen
5. **Keine Heilversprechen** in Texten — juristische Vorsicht bei Produktbeschreibungen
6. **WhatsApp-Link** Format: `https://wa.me/49XXXXXXXXX` (Nummer einsetzen)
7. **Bilder** immer mit `loading="lazy"` außer Hero-Bild
8. **Performance:** Bilder vor dem Deployment optimieren (max 200KB pro Bild)

---

## Deployment

**Workflow:**
1. Änderung in `index.html` machen
2. `git add . && git commit -m "beschreibung"` 
3. `git push` → GitHub Pages deployed automatisch
4. Hostinger-Domain zeigt auf GitHub Pages (CNAME bereits eingerichtet)

**GitHub Repo:** (URL hier eintragen nach Setup)  
**Live URL:** (Domain hier eintragen)

---

## Offene To-Dos

- [ ] WhatsApp-Nummer eintragen (alle `wa.me/` Links)
- [ ] Echte Fotos von Giuseppina einbinden (statt Placeholder)
- [ ] Impressum & Datenschutz Seite erstellen (rechtlich notwendig!)
- [ ] GitHub Repo erstellen und GitHub Pages aktivieren
- [ ] Hostinger-Domain auf GitHub Pages zeigen lassen
- [ ] Google Analytics / Meta Pixel einbinden (optional)
- [ ] Echte Kundenbewertungen eintragen

---

## Wichtige Hinweise

- **Impressum ist Pflicht** in Deutschland — ohne geht die Seite nicht live
- **Datenschutzerklärung** ist Pflicht (DSGVO) — besonders wenn Formulare genutzt werden
- **LR Health & Beauty** ist ein MLM-Unternehmen — keine irreführenden Einkommensversprechen auf der Seite
