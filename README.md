# Lanka Tiles PLC — Visitor Management System

A fully offline, browser-based Visitor Management System for Lanka Tiles PLC.  
Hosted free on **GitHub Pages** — no server required.

## 🌐 Live URL

After enabling GitHub Pages, your site will be at:  
`https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

## ✨ Features

- Pre-registration (individual & group with drivers)
- Guardroom check-in / check-out with pass issuance
- Colour-coded access zones (Green / Yellow / Amber / Red)
- Photography/Videography permission tracking
- NIC/Passport validation
- Admin panel (hosts, zones, pass totals)
- Export to Excel / CSV
- **☁ GitHub Gist Sync** — optional automatic cloud backup

## 💾 Data Storage

All data is stored in the **browser's localStorage** on the device used.  
To prevent data loss, set up **GitHub Gist Sync** (free):

1. Open the app → **Admin** → **GitHub Gist Sync** → **Configure**
2. Create a GitHub Personal Access Token (gist scope only)
3. Create a secret Gist named `vms_data.json`
4. Enter both in the settings — data auto-syncs after every change

## 🚀 How to Deploy (one-time setup)

1. Create a new GitHub repository (public or private)
2. Upload all files in this folder to the repository root
3. Go to **Settings** → **Pages** → Source: **Deploy from branch** → Branch: `main` → folder: `/ (root)`
4. Click **Save** — site goes live in ~60 seconds

## 📁 Files

| File | Purpose |
|------|---------|
| `index.html` | The entire application (single file) |
| `_config.yml` | GitHub Pages configuration |
| `.nojekyll` | Prevents Jekyll processing (required) |
| `README.md` | This file |

## 🔒 Notes

- Data lives in the browser — **use one device** or set up Gist sync
- Admin password default: `lanka2026` (change in Admin → Settings)
- Works offline after first load (browser caches the page)
