
# GlassFin — Modular glassy theme for Jellyfin (Dark, Nord, Neon, TV flavors)

## How to use
1) Host the folder contents on any static server (Nginx, GitHub Pages, etc.).
2) In Jellyfin:
   - Server-wide: Dashboard → General → Branding → Custom CSS
   - Per user: Settings → Display → Custom CSS (optionally tick "Disable server-provided custom CSS").
3) Paste ONE of these in "Custom CSS":
   - Base + Dark (recommended start):
     @import url("https://YOUR.CDN/GlassFin/GlassFin-oneliner.css");
   - Or manual selection:
     @import url("https://YOUR.CDN/GlassFin/GlassFin-main.css");
     @import url("https://YOUR.CDN/GlassFin/GlassFin-Extras.css");
     @import url("https://YOUR.CDN/GlassFin/GlassFin-Icons.css");
     @import url("https://YOUR.CDN/GlassFin/Themes/GlassFin-Dark.css");

## Fonts
- Place your "ArslanWessamB.woff2" under ./fonts and uncomment the @font-face block in GlassFin-main.css.
- Included fallback from your upload: KFGQPC-Uthmanic-HAFS-Regular.woff2 (note: decorative, not ideal for general UI).

## Notes
- Blur is disabled automatically on TV flavor to improve performance.
- Provider icons are shipped as simple badges first (fast, accessible). If you want SVG logos, I can add them next.
