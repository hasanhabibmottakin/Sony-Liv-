<h1 align="center">🔁 Auto Update Sony Events</h1>

<p align="center">
  <img src="[https://upload.wikimedia.org/wikipedia/commons/4/4d/SonyLIV_logo.svg](https://etimg.etb2bimg.com/photo/76029910.cms)" alt="SonyLIV" width="200"/>
</p>

<p align="center">
  <b>Automatically fetches and updates the latest SonyLIV event playlist every 10 minutes.</b><br>
  <sub>Powered by <b>GitHub Actions</b> & maintained by <b>BD Coder Boy</b></sub>
</p>

---

### ⚙️ Overview

This repository uses **GitHub Actions** to automatically update:
- 🎬 `playlist.m3u` — a valid M3U playlist of SonyLIV live events.
- 🧾 `sony_event.json` — JSON-formatted metadata of all active Sony events.

Updates are performed **every 10 minutes**, ensuring your event list always stays fresh and accurate.

---

### 🚀 Features
.  
✅ Extracts event metadata: name, logo, category, language, and stream URL.  
✅ Builds both `.m3u` and `.json` outputs automatically.  
✅ Commits and pushes updates using GitHub Actions bot.  
✅ Runs fully serverless — no manual setup required.

---

### 🧩 Output Files

| File | Description |
|------|--------------|
| `playlist.m3u` | Ready-to-use SonyLIV playlist with correct User-Agent headers. |
| `sony_event.json` | JSON API of all events with full metadata. |

---

