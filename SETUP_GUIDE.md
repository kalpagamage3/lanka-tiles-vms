# 📋 GitHub Pages Setup Guide — Lanka Tiles VMS

## Step 1 — Create GitHub Account (if you don't have one)
Go to https://github.com and sign up for free.

## Step 2 — Create a New Repository

1. Click the **+** button (top right) → **New repository**
2. Name it anything, e.g. `lanka-tiles-vms`
3. Set to **Private** (recommended for security)
4. Leave all other options as default
5. Click **Create repository**

## Step 3 — Upload Files

1. On the new repository page, click **uploading an existing file**
2. Drag and drop ALL files from this folder:
   - `index.html`
   - `_config.yml`
   - `.nojekyll`
   - `README.md`
   - `404.html`
   - `SETUP_GUIDE.md`
3. Scroll down → click **Commit changes**

   ⚠️ Make sure `.nojekyll` is uploaded — it might be hidden on your computer.
   On Windows: View → Show hidden files.
   On Mac: Cmd+Shift+. to show hidden files.

## Step 4 — Enable GitHub Pages

1. In your repository, go to **Settings** (top menu)
2. In the left sidebar, scroll to **Pages**
3. Under **Source**, select:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **Save**
5. Wait about 60 seconds, then refresh the page
6. You'll see: "Your site is live at https://USERNAME.github.io/REPONAME/"

## Step 5 — Access the System

Open the URL shown on the Pages settings page.
Share this URL with factory employees on any device.

---

## ☁ Optional: Set Up Auto-Backup to GitHub Gist

This keeps your data safe even if the browser cache is cleared.

### Create a Gist

1. Go to https://gist.github.com
2. Filename: `vms_data.json`
3. Content: `{}`
4. Click **Create secret gist**
5. Copy the Gist ID from the URL:
   `https://gist.github.com/USERNAME/`**`abc123def456...`** ← this part

### Create a Personal Access Token

1. Go to https://github.com/settings/tokens
2. Click **Generate new token (classic)**
3. Name: `VMS Gist Backup`
4. Check only: ☑ **gist**
5. Click **Generate token**
6. Copy the token (starts with `ghp_...`) — you only see it once!

### Configure in VMS

1. Open the VMS app
2. Go to **Admin** panel (password: `lanka2026`)
3. Find **GitHub Gist Sync** section
4. Click **Configure**
5. Paste your token and Gist ID
6. Set auto-sync interval (e.g. `5` minutes)
7. Click **Save Settings**
8. Click **Test Sync Now** to verify

Data now auto-syncs to GitHub after every change.
To restore data on a new device, go to Admin → Gist Sync → Restore from Gist.

---

## 🔑 Important Notes

| Setting | Value |
|---------|-------|
| Admin password | `lanka2026` (change this!) |
| Data storage | Browser localStorage (this device only) |
| Backup | GitHub Gist (if configured) |
| Cost | Free (GitHub Pages free tier) |
| Users | Unlimited devices can VIEW the site |

## ❓ Troubleshooting

**Site shows "404 Not Found"**
→ GitHub Pages takes up to 5 minutes to activate. Wait and refresh.

**Page shows raw code**
→ Make sure `.nojekyll` file was uploaded correctly (it has no extension).

**Data disappeared after refresh**
→ Set up GitHub Gist Sync to keep data safe across sessions.

**Admin password not working**
→ Default is `lanka2026` — check you're using the correct device
  (data and password are stored per-browser).
