# Story Cards

Write and time video scripts, scene by scene. Runs entirely in the browser,
saves to the device it's on, and installs like a real app. No build step, no
framework, no backend — one folder of static files.

**Live:** _(add your hosted link here)_

---

## What's in this folder

| | |
|---|---|
| `index.html` | the app (open this one) |
| `manifest.webmanifest` | makes it installable |
| `sw.js` | service worker (works offline) |
| `icon.svg` / `*.png` | app icons |
| `fonts/` | Jost (SIL Open Font License) |

Keep these together — the whole folder is the app.

## Run it locally

It's static, so any web server works:

```bash
npx serve .        # then open the printed http://localhost… URL
```

(Opening `index.html` directly with `file://` mostly works, but a server is
needed for the install/offline features.)

## Put it online (≈2 minutes)

1. Open **app.netlify.com/drop**.
2. Drag this folder onto the page.
3. You get a link like `your-name.netlify.app`.

GitHub Pages, Vercel, and Cloudflare Pages work too — point them at this folder.

## Use it like an app

- **iPhone (Safari):** Share → "Add to Home Screen".
- **Android (Chrome):** ⋮ → "Install app".
- **Laptop (Chrome/Edge):** Install icon in the address bar. **Safari (macOS):** File → "Add to Dock".

Launches fullscreen, its own icon, works offline.

## Your data — private by design

Everything is stored in **your browser, on your device** (localStorage). It is
never uploaded anywhere, so if others use the hosted app, their writing stays
on their devices and yours stays on yours. The trade-off: your own devices
don't auto-sync. Move work between them with the pencil menu:

- **Save to file** — writes a backup file you own (on Chrome/Edge, re-saving
  silently overwrites the same file).
- **Open backup file** — load it back, here or on another device.
- **Export document (.doc)** — a formatted script to share/print.

## Credits

- Design inspired by **Anton — [halfof8.com](https://halfof8.com)**.
- Typeface: **Jost** (Owen Earl), SIL Open Font License.
- Open software (MIT, see `LICENSE`). Not affiliated with any brand.
