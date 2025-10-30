# Personal Portal (HTML/JS)

A single-file, browser-based portal. Enter a name, DOB (auto age), create custom **sections** (each with attachments + notes), and manage **Calendar** events. Everything is stored locally in your browser via IndexedDB. Export/Import a backup JSON anytime.

## Use
Open `index.html` in any modern browser.

- **Add Section** to create a new tab (e.g., “Insurance”, “Education”).  
- Each section supports drag-and-drop file attachments, open/download/remove, and notes.  
- **Calendar**: create, edit, delete events; export a single event or an entire month as `.ics`.  
- **Backup**: exports all sections, files (as base64), notes, events, and profile.  
- **Restore**: imports from a prior backup JSON.

## GitHub Pages
1. Create a repo and add `index.html` (and this README if you want).
2. Commit & push.
3. In **Settings → Pages**, set **Source: Deploy from a branch**, pick `main` and `/ (root)`.
4. Open the Pages URL to use the portal online (data stays in the browser; it’s not uploaded).

> Tip: If you serve from `file://` locally and your browser blocks IndexedDB, use a local server
> (e.g., `python -m http.server` in the folder) or GitHub Pages.
