# Luceo Practice Plan Builder

Builds a practice plan, runs it live on a tablet, and tracks the season.

Open the live builder: **https://ericweiss-ls.github.io/practice-plan-builder/**

- `index.html` is the whole app. One self-contained file.
- `manifest.webmanifest`, `sw.js` and the icons make it installable on an iPad (Share → Add to Home Screen) and let it open offline after the first load.

## Updating

Replace `index.html` and push to `main`. GitHub Pages republishes within a minute or two; people who have the page open get the new version on their next reload. The service worker is network-first, so a reload is enough.

## Notes

- Plans, results and the team setup are stored in the browser on each person's own device. Use Backup (shared Google Drive folder) to move them between devices and coaches.
- The app opens empty and asks for the head coach's name. Drills and plays build themselves as you write plans; Team › Team file saves the whole setup to move to another device. Menu (⋯) › **Load demo data** adds a sample team and five practices; **Clear demo data · start fresh** removes them again.
- Playbook and Drill Library import icons are placeholders until the Luceo app connects.
