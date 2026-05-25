# 🎮 GameFinder

**Dein Gaming-Portal** – Suche nach Spieletipps, Cheats, Videos, Walkthroughs & Downloads für alle Gaming-Plattformen.

![GameFinder Screenshot](https://via.placeholder.com/800x400/050508/00f5d4?text=GameFinder)

---

## ✨ Features

- 🔍 **Spielesuche** mit Autovervollständigung (powered by RAWG.io – 500.000+ Spiele)
- 🎯 **Plattform-Filter** – Hierarchisch: Hersteller → Konsole
  - PC (Windows, macOS, Linux)
  - Sony (PS1 bis PS5, PSP, PS Vita)
  - Nintendo (NES bis Switch, alle Handhelds)
  - Microsoft (Xbox bis Xbox Series X/S)
  - Sega (Master System bis Dreamcast)
  - Atari, Mobile (iOS/Android)
- 📂 **6 Kategorien**: Tipps & Tricks, Cheats, Videos, Blogs/Reviews, Downloads/Mods, Walkthroughs
- 💾 **Lokale Spieldatenbank** mit Update-Funktion (IndexedDB via localStorage)
- 🌓 **Dark Gaming UI** – Neon-Cyan & Lila, vollständig responsiv
- 📱 **PWA** – Als App auf dem Homescreen installierbar

---

## 🚀 Deployment auf GitHub Pages

### 1. Repository klonen / Dateien hochladen

```bash
git clone https://github.com/reneprause-dot/gamefinder.git
cd gamefinder
# Alle Dateien in dieses Verzeichnis kopieren
git add .
git commit -m "🎮 Initial GameFinder release"
git push origin main
```

### 2. GitHub Pages aktivieren

1. Gehe zu deinem Repository auf GitHub
2. **Settings** → **Pages**
3. Source: **Deploy from a branch**
4. Branch: **main** / Root: **/ (root)**
5. **Save** klicken
6. Nach 1-2 Minuten ist die App unter `https://reneprause-dot.github.io/gamefinder` erreichbar

---

## 🔑 API Keys

| Service | Key | Limits |
|---------|-----|--------|
| [RAWG.io](https://rawg.io/apidocs) | Im Code hinterlegt | 20.000 req/Monat (kostenlos) |

---

## 📁 Projektstruktur

```
gamefinder/
├── index.html          # Haupt-App
├── manifest.json       # PWA Manifest
├── css/
│   └── style.css       # Alle Styles
├── js/
│   ├── platforms.js    # Plattform-Datenbank & Suchdefinitionen
│   └── app.js          # Hauptlogik, RAWG-Integration
├── icons/
│   ├── icon-192.png    # PWA Icon
│   └── icon-512.png    # PWA Icon (groß)
└── README.md
```

---

## 🛠 Technologien

- **Vanilla HTML/CSS/JS** – keine Build-Tools, keine Dependencies
- **RAWG.io API** – Spieledatenbank & Metadaten
- **localStorage** – Lokale Spieledatenbank (bis ~5MB)
- **CSS Grid + Flexbox** – Responsives Layout
- **Google Fonts** – Orbitron, Rajdhani, JetBrains Mono

---

## 📝 Lizenz

MIT – frei verwendbar und veränderbar.
