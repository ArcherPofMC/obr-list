# Technique Search — Owlbear Rodeo Extension

A keyword search panel for use directly in Owlbear Rodeo.


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


