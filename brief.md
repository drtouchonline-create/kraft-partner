# Brief — Kraft GmbH Website Modernisierung

**Auftraggeber:** Kraft GmbH, München  
**Auftragnehmer:** Touch Digital  
**Kontakt:** njasik@icloud.com  
**Datum:** 2026-05  
**Status:** Proposal → Umsetzung offen

---

## Projektziel

Kraft GmbH ist der einzige IT-Spezialist für den gesamten deutschen Leasing-Software-Stack. Dieses Alleinstellungsmerkmal ist auf der aktuellen Website unsichtbar. Ziel ist eine vollständige digitale Neupositionierung:

- **Mehr Kundenanfragen** über automatisierte Lead-Kanäle
- **Professioneller Auftritt** vor Banken und Großunternehmen
- **Google-Sichtbarkeit** für Nischen-Suchanfragen ohne Wettbewerb
- **Autorität** als Nr. 1 im deutschen Leasing-IT-Markt

---

## Ausgangslage

**Website:** kraft-partner.com  
**Probleme:**
- Veraltetes Design (~2012)
- Keine CTAs, kein Kontaktformular
- Kein Social Proof (keine Kundenstimmen, keine Logos)
- Kein SEO / kein Blog
- Schwache Mobile-Optimierung
- Kein Chatbot, kein Terminbuchungs-Widget
- Keine klare Positionierung vs. Wettbewerber

---

## Technischer Stack

| Parameter | Wert |
|-----------|------|
| Technologie | HTML / CSS / JS (Vanilla) |
| Hosting | Vercel (bereits konfiguriert) |
| Externe Libraries | Keine CDN — nur Google Fonts |
| Sprache | Deutsch (Primär), Englisch (Phase 2) |
| Design-System | Navy/Gold, Playfair Display + DM Sans |
| Datei | Einzelne `index.html` (self-contained) |

---

## Module — Priorität Hoch (Wochen 1–2)

### 1. Modernes Redesign
- Hero-Bereich mit animiertem Gradient-Titel
- Sticky Navbar mit Hamburger-Menü (mobil)
- Scroll-Reveal Animationen (fade bottom / left / right)
- Parallax-Hintergrundbild
- Floating Gold-Partikel im Hero

### 2. Online-Terminbuchung
- Eingebettetes Widget (Calendly oder eigenes)
- Direkt in der CTA-Sektion
- Mobile-optimiert

### 3. Kontaktformular
- Felder: Name, E-Mail, Nachricht
- Validierung (client-side)
- Erfolgs-Animation: SVG-Checkmark (Draw-on-Appear)
- Backend: Formspree oder Netlify Forms

### 4. Vertrauen & Social Proof
- Kundenstimmen-Slider
- Partner-Logos (Leasing-Software-Hersteller)
- Kennzahlen: 27 Jahre, X Projekte, X Länder

---

## Module — Priorität Mittel (Monat 1–2)

### 5. Interaktiver Kosten-Kalkulator
- 4–5 Schritt-Quiz: System → Datenmenge → Projekttyp → Ergebnis
- Lead-Capture: E-Mail für Ergebnis-Zustellung
- Stack: JS + LocalStorage, kein Backend nötig

### 6. KI-Chatbot
- Basis: Claude API (claude-haiku-4-5-20251001)
- Persona: „Kraft Assistent"
- Kann beantworten: Systemfragen, Services, Termin buchen
- Sprache: Deutsch

### 7. DORA / NIS2 Landingpage
- Dedizierte URL: `/dora-compliance`
- Argument: IT-Modernisierung = regulatorische Pflicht
- CTA: Kostenloses Erstgespräch

### 8. Marktpositionierungs-Seite
- „Nr. 1 im Leasing" Seite
- Vollständiger Software-Stack visuell dargestellt
- Competitor-Vergleichstabelle

---

## Module — Phase 2 (Monat 3–6)

### 9. SEO-Blog
- CMS: Sanity oder Contentlayer
- Ziel-Keywords: „NAVILEASE Migration Partner", „Datenmigration Leasinggesellschaft", „DORA Compliance Leasing IT"
- Veröffentlichungsrhythmus: 2× pro Monat

### 10. Kunden-Portal
- Login-Bereich für aktive Kunden
- Projekt-Tracking: Status, Meilensteine, Dokumente
- Stack: Next.js + Supabase Auth

### 11. E-Mail-Automatisierung
- Tool: Brevo (ex-Sendinblue) oder HubSpot Free
- Sequenz: Anfrage → Danke → Case Studies → Follow-up

### 12. Mehrsprachigkeit DE/EN
- i18n: JSON-basierte Übersetzungen
- URL-Struktur: `/en/` Subdirectory

---

## Design-Anforderungen

```
Farben:
  --navy:   #01030a  (Hintergrund dunkel)
  --navy2:  #060f1f  (Sektionen hell)
  --gold:   #c9a84c  (Akzentfarbe)
  --gold2:  #e8c96a  (Hover / Highlights)
  --white:  #ffffff

Schriften:
  Playfair Display 700/900  → Überschriften
  DM Sans 300/400/500/600   → Fließtext

Abstände:
  Section padding: 100px (Desktop), 72px (Tablet), 60px (Mobile)
  Max-Width: 1200px

Breakpoints:
  Mobile:  < 480px
  Tablet:  480px – 768px
  Desktop: > 768px
```

---

## Lieferumfang (Phase 1)

| # | Deliverable | Status |
|---|-------------|--------|
| 1 | `index.html` — Lendingpage mit Animationen | ✅ Fertig |
| 2 | Navbar + Hamburger-Menü | ✅ Fertig |
| 3 | Scroll Reveal + Parallax + Partikel | ✅ Fertig |
| 4 | Kontaktformular mit Erfolgs-Animation | ✅ Fertig |
| 5 | Back-to-Top Button | ✅ Fertig |
| 6 | Counter-Animationen | ✅ Fertig |
| 7 | 3D-Tilt auf Karten | ✅ Fertig |
| 8 | Button Shimmer-Effekte | ✅ Fertig |
| 9 | Foto-Platzhalter (hero-bg.jpg, team.jpg) | ⏳ Fotos ausstehend |
| 10 | Vercel Deployment | ✅ Konfiguriert |

---

## Fotos (ausstehend)

Bitte folgende Dateien in den Ordner `images/` legen:

| Datei | Inhalt | Größe |
|-------|--------|-------|
| `images/hero-bg.jpg` | Dunkles Büro, Bankgebäude oder München Nacht | 1920 × 1080 px |
| `images/team.jpg` | Touch Digital Team oder professionelles Bürofoto | 800 × 600 px |

---

## Nächste Schritte

1. [ ] Fotos einfügen (`images/hero-bg.jpg`, `images/team.jpg`)
2. [ ] Terminbuchungs-Widget integrieren (Calendly-Link)
3. [ ] Formular-Backend verbinden (Formspree / Netlify Forms)
4. [ ] Kalkulator-Modul entwickeln
5. [ ] KI-Chatbot integrieren (Claude API)
6. [ ] DORA-Landingpage erstellen
7. [ ] SEO-Blog Struktur aufbauen

---

*Erstellt von Touch Digital · njasik@icloud.com · touchdigital.de*
