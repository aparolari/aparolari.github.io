# Parolari Ecohydrology Lab Website

Website for the [Ecohydrology @ Marquette](https://www.aphydro.com) research lab, hosted on GitHub Pages.

## 🚀 How to Deploy on GitHub Pages

### Step 1 — Create a GitHub account (if you don't have one)
Go to [github.com](https://github.com) and sign up.

### Step 2 — Create a new repository
- Click the **+** icon → **New repository**
- Name it: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
  - For example: `aparolari.github.io`
- Set visibility to **Public**
- Click **Create repository**

### Step 3 — Upload your files
**Option A — Via the GitHub website (easiest):**
1. In your new repo, click **Add file** → **Upload files**
2. Drag and drop `index.html` into the upload area
3. Click **Commit changes**

**Option B — Via Git (command line):**
```bash
git clone https://github.com/yourusername/yourusername.github.io
cd yourusername.github.io
cp /path/to/index.html .
git add index.html
git commit -m "Initial site"
git push origin main
```

### Step 4 — Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages** (left sidebar)
2. Under **Source**, select **Deploy from a branch**
3. Set branch to `main` and folder to `/ (root)`
4. Click **Save**

### Step 5 — Your site is live! 🎉
Within 1–2 minutes, your site will be live at:
`https://yourusername.github.io`

---

## 🌐 Using a Custom Domain (aphydro.com)

To keep your `aphydro.com` domain instead of the GitHub URL:

1. In your repo, create a file called `CNAME` (no extension) containing just:
   ```
   www.aphydro.com
   ```
2. In your domain registrar (Squarespace Domains or wherever aphydro.com is registered), update the DNS:
   - Add a `CNAME` record: `www` → `yourusername.github.io`
   - Or set `A` records to GitHub's IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. In GitHub Pages Settings → **Custom domain**, type `www.aphydro.com` and save
4. Check **Enforce HTTPS** once DNS propagates (can take up to 48 hours)

---

## ✏️ How to Update the Site

All content lives in `index.html`. Open it in any text editor and:
- **Update publications**: Find the `<ol class="pub-list">` section and add new `<li class="pub-item">` entries at the top
- **Add a student**: Copy a `<div class="student-card">` block and fill in the details
- **Update courses**: Edit the course items in the `#teaching` section
- **Change your bio**: Find the `<div class="pi-info">` block

After editing, re-upload `index.html` to GitHub and the site updates automatically.

---

## 📁 File Structure

```
yourusername.github.io/
├── index.html    ← The entire website (single file)
├── README.md     ← These instructions
└── CNAME         ← (optional) for custom domain
```
