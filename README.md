# Technique Search — Owlbear Rodeo Extension

A keyword search panel for Phantasy Star (SkyDawn Games) techniques, embedded directly in Owlbear Rodeo.

## How to use
- Click the search icon (🔍) in the top-left action bar of your OBR room
- Type a technique name (or partial name) to find it instantly
- Each result shows Rank, Classes, Cast Time, Range, Effect, and Notes
- Click **✕** on any card to dismiss it
- Click **✕** next to the search bar to clear and start over

---

## Hosting on GitHub Pages (free, recommended)

1. Create a new repository on GitHub (e.g. `technique-search`)
2. Upload all files in this folder: `manifest.json`, `index.html`, `icon.svg`
3. Go to **Settings → Pages** and set source to `main` branch, `/ (root)`
4. GitHub will give you a URL like: `https://yourusername.github.io/technique-search/`
5. Your manifest URL will be: `https://yourusername.github.io/technique-search/manifest.json`

## Installing in Owlbear Rodeo

1. Go to your OBR profile → **Add Extension**
2. Paste your manifest URL and click Add
3. When creating or opening a room, enable the extension in the room settings
4. The search icon will appear in the top-left action bar

---

## Adding more techniques later

Open `index.html` and find the `TECHNIQUES` array near the top of the `<script>` block.
Add new entries following this format:

```js
{ name:"Technique Name", rank:"1", classes:"Guardian, Hunter", castTime:"Action", range:"60 ft.", effect:"Your effect text here.", notes:"Optional notes" },
```

Rank values: `"Prime"`, `"1"` through `"9"`

When you save and push to GitHub, the extension updates automatically for all rooms using it.
