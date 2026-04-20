<div align="center">

# SeerFin

**A Jellyfin theme inspired by Jellyseerr**

[![Version](https://img.shields.io/badge/version-1.0.0-orange?style=flat-square)](https://github.com/tardisjellyshowrunner/SeerFin/releases)
[![Jellyfin](https://img.shields.io/badge/Jellyfin-10.9%2B-00A4DC?style=flat-square&logo=jellyfin&logoColor=white)](https://jellyfin.org)
[![License](https://img.shields.io/badge/license-MIT-purple?style=flat-square)](LICENSE)
[![jsDelivr](https://img.shields.io/badge/CDN-jsDelivr-E84D3D?style=flat-square)](https://cdn.jsdelivr.net/gh/tardisjellyshowrunner/SeerFin@main/Theme/release/SeerFin.css)

SeerFin brings the look and feel of [Jellyseerr](https://github.com/seerr-team/seerr) to your Jellyfin media server. Dark navy backgrounds, orange accent colours, purple/indigo active states, and clean DM Sans typography — all in a single CSS import.

</div>

---

## ✨ Features

- 🎨 **Jellyseerr palette** — Tailwind gray-900/800/700 navy backgrounds (`#111827` base) with orange-500 (`#f97316`) accents
- 💜 **Purple/indigo active states** — Navigation pill states matching Jellyseerr's UI exactly
- 🔤 **DM Sans typography** — Clean, modern font replacing Jellyfin's default
- 🃏 **Refined card design** — Rounded corners, subtle borders, smooth hover transitions
- 📱 **Mobile, desktop & TV** — Single import works across all Jellyfin layouts
- 🎬 **Video player friendly** — Compatible with Jellyfin's video player, subtitle rendering, and OSD controls
- 🖱️ **Custom scrollbars** — Slim dark scrollbars with orange hover state
- ⚙️ **Fully customisable** — All colours exposed as CSS variables for easy overrides

---

## 📸 Screenshots

> Screenshots coming soon. Contributions welcome — see [Contributing](#contributing).

---

## 🚀 Installation

### Jellyfin Web (Desktop/Mobile)

1. Open Jellyfin and sign in
2. Go to **Settings** → **Display**
3. Scroll to **Custom CSS**
4. Paste the following and click **Save**:

```css
@import url("https://cdn.jsdelivr.net/gh/tardisjellyshowrunner/SeerFin@main/Theme/release/SeerFin.css");
```

5. Refresh the page

### Jellyfin Dashboard (Admin)

1. Go to **Dashboard** → **Administration** → **Branding**
2. Paste the import into the **Custom CSS** box
3. Click **Save**

> **Note:** The CDN may take a few minutes to serve a newly updated file. If you see no change after saving, try a hard refresh (`Cmd+Shift+R` / `Ctrl+Shift+R`).

---

## 🎨 Colour Palette

| Role | Colour | Hex |
|------|--------|-----|
| Background base | ![#111827](https://placehold.co/12x12/111827/111827.png) Navy | `#111827` |
| Surface | ![#1f2937](https://placehold.co/12x12/1f2937/1f2937.png) Dark navy | `#1f2937` |
| Elevated | ![#374151](https://placehold.co/12x12/374151/374151.png) Mid navy | `#374151` |
| Accent primary | ![#f97316](https://placehold.co/12x12/f97316/f97316.png) Orange | `#f97316` |
| Active state | ![#6366f1](https://placehold.co/12x12/6366f1/6366f1.png) Indigo | `#6366f1 → #8b5cf6` |
| Secondary accent | ![#2dd4bf](https://placehold.co/12x12/2dd4bf/2dd4bf.png) Teal | `#2dd4bf` |
| Text primary | ![#e5e7eb](https://placehold.co/12x12/e5e7eb/e5e7eb.png) Light grey | `#e5e7eb` |
| Text muted | ![#9ca3af](https://placehold.co/12x12/9ca3af/9ca3af.png) Mid grey | `#9ca3af` |

---

## 🔧 Customisation

All design tokens are exposed as CSS variables in `:root`. To override any value, append your own CSS after the import:

```css
@import url("https://cdn.jsdelivr.net/gh/tardisjellyshowrunner/SeerFin@main/Theme/release/SeerFin.css");

:root {
  /* Change the primary accent from orange to blue */
  --sf-accent: #3b82f6;
  --sf-accent-hover: #60a5fa;

  /* Change the active pill gradient */
  --sf-active-from: #0ea5e9;
  --sf-active-to: #6366f1;
}
```

---

## ⚠️ Known Issues

| # | Issue | Status |
|---|-------|--------|
| [#9](https://github.com/tardisjellyshowrunner/SeerFin/issues/9) | Video player dialogs (cast, group play, subtitles, settings) apply a dark overlay that hides the video when opened | 🔴 Open |
| [#10](https://github.com/tardisjellyshowrunner/SeerFin/issues/10) | Top OSD bar (episode title / controls) renders as a solid block rather than a transparent gradient overlay during playback | 🔴 Open |

---

## 📁 Repository Structure

```
SeerFin/
├── Theme/
│   ├── release/
│   │   └── SeerFin.css          ← Stable release (use this)
│   └── dev/
│       └── seerfin-v*.css       ← Development versions
└── README.md
```

---

## 🙏 Acknowledgements

- **[ElegantFin](https://github.com/lscambo13/ElegantFin)** by lscambo13 — structural foundation and background handling approach
- **[Jellyseerr](https://github.com/seerr-team/seerr)** by the Seerr Team — design inspiration and colour palette
- **[JellySkin](https://github.com/prayag17/JellySkin)** by prayag17 — addon architecture reference
- **[Jellyfin](https://jellyfin.org)** — the open source media server this theme is built for

---

## 📄 License

MIT © [tardisjellyshowrunner](https://github.com/tardisjellyshowrunner)

---

<div align="center">

Made with ☕ and too many browser DevTools sessions

</div>
