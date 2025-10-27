<h1 align="center">🔁 Auto Update Sony Events</h1>

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4d/SonyLIV_logo.svg" alt="SonyLIV" width="200"/>
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

✅ Auto-fetches SonyLIV playlist from a secure URL (stored as GitHub Secret).  
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

### 🔑 Secrets Configuration

Add the following secret in your repository:

| Name | Description |
|------|--------------|
| `URL` | The secure playlist URL to fetch Sony event data from. |

---

### 🕒 Cron Schedule

This action runs automatically **every 10 minutes**:

```yaml
on:
  schedule:
    - cron: "*/10 * * * *"
