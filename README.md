# alessioaretano.com

Persönliche Link-in-Bio-Seite von Alessio Aretano (Endurance Athlete).
Statische Single-Page, gehostet über **GitHub Pages** unter der Custom-Domain
[alessioaretano.com](https://alessioaretano.com).

Design: *Kinetic Velocity* — Dark Glassmorphism + Athletic Minimalism
(Volt-Grün `#C3FF00`, Cyber-Blau `#00B3FF`, Fonts Sora / Inter / JetBrains Mono).

## Aufbau

```
index.html      → komplette Seite (HTML + CSS + JS, selbst-enthalten, kein Build nötig)
assets/avatar.jpg  → Profilfoto
assets/hero.jpg    → unscharfer Hintergrund (Motion-Blur-Run)
assets/og.jpg      → Social-Preview-Bild (Open Graph / Twitter)
CNAME           → Custom-Domain für GitHub Pages
favicon         → inline im <head> (Volt-Grün „A")
```

## Inhalte ändern

Alles in `index.html`:

- **Links / Codes** → `<div class="links">` (Affiliate-Buttons) und `<nav class="social">` + `<footer>`.
- **Stats** → `<div class="stats">` (Weekly Volume / Max Duration).
- **Fotos** → Datei in `assets/` ersetzen (Name beibehalten) oder Pfad im HTML anpassen.

## Lokal ansehen

```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## Deploy

Push auf `main` → GitHub Pages baut automatisch (≈1 Min). Quelle: Branch `main`, Ordner `/` (root).
