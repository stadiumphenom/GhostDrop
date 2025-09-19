# 👻 GhostDrop

**Invisible sync, visible results.**

GhostDrop is a lightweight Dropbox → GitHub pipeline.  
Drop your files in Dropbox → they commit themselves to GitHub. No manual uploads, no context switching.

---

## 🚀 Features
- One-time setup with tokens + repo mapping (`repos.json`)
- Auto-sync Dropbox folders → GitHub repos
- Handles file updates + deletes
- SQLite-backed state (resilient to crashes)
- Webhook support for near real-time sync

---

## 🛠️ How It Works
1. Add your tokens in `ghostdrop/`:
   - `dropbox token.txt`
   - `dropbox secret.txt`
   - `github token.txt`
   - `repos.json`

2. Run the sync service:
   ```bash
   python dropbox_github_multi_sync.py
