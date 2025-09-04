# Twins Daily Log

Single-file daily log for twins. Track feeds, diapers, sleep, pumping, and notes. Works offline in the browser and keeps data on your device (LocalStorage). Export CSV or print a paper copy.

**Live site:** https://twinsdailylog.netlify.app/

---

## Features
- 🍼 Track: feed type/oz/min, diaper (W/S/B), sleep (start–end), pump (oz/min), notes
- 👶 Custom child names (Twin A/B) + per-entry name override
- 🧮 Daily totals bar: fed oz, pumped oz, diaper counts, total sleep hh:mm
- ✏️ Edit & delete entries
- 🌙 Dark mode toggle
- 🇺🇸/🇪🇸 English/Spanish toggle
- 🗓️ Prev/Next day controls
- 📄 Print-friendly layout
- 📤 CSV export (see columns below)
- 💾 LocalStorage only (no server/database)

## Quick Start
1. Open the live site or download `index.html` and double-click to run locally.
2. Set names in **Totals → Names** (saved to your browser).
3. Add entries; use **Edit/Delete** as needed.
4. **Export CSV** for sharing or backups; **Print** for paper logs.

## CSV Columns
`Date, Time, TwinId, ChildName, FeedType, FeedOz, FeedMin, PumpOz, PumpMin, Diaper(W/S/B), SleepStart, SleepEnd, Notes`

## Deploy
### Netlify (manual)
- Netlify → *your site* → **Deploys → Upload deploy** → upload a folder/ZIP whose **top level contains `index.html`**.

### Netlify (from GitHub)
- Site settings → **Build & deploy → Continuous Deployment** → connect this repo.
- Build command: *(leave empty)*, Publish directory: **/** (repo root).
- Every commit to `main` redeploys automatically.

## Update Tips
- Replace `index.html` and redeploy.
- If the site looks unchanged, open with a cache-buster query (e.g., `?v=12`) or hard-refresh.

## Privacy
- All data is stored locally in your browser’s **LocalStorage**. Clearing site data, using a different device, or private/incognito mode will reset the log. Export CSV to keep backups.

## Troubleshooting
- **404 or blank page:** ensure `index.html` is at the **root** of the deploy (not inside a subfolder).
- **Windows saved `index.html.html`:** enable file-name extensions and rename to `index.html`.
- **Changes not visible:** try Incognito or append `?v=timestamp` to the URL.

## License
Choose what you prefer:
- **MIT** (permissive; great for sharing), or
- “All rights reserved” (private use).

