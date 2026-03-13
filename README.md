# 📊 Meta Report Generator · kajgod.agency

A fully client-side monthly report generator that connects directly to **Meta Business Suite via the Graph API** — no manual CSV exports, no backend, no cost.

Your client logs in once with Facebook, selects the page and month, and the app pulls all metrics automatically and generates a branded PDF.

---

## ✨ What it does

- **Live Meta API connection** — pulls real data from Facebook & Instagram automatically
- **No manual exports** — replaces the .xlsx download workflow entirely
- **Multi-platform** — Facebook Pages + linked Instagram Business accounts
- **Branded PDF output** — kajgod.agency visual identity on every report
- **One-click generate** — select month → click generate → download PDF
- **Zero backend** — runs entirely in the browser, nothing stored on any server

---

## 🚀 Setup (~15 minutes, one-time)

### 1 — Create a Meta Developer App
Go to [developers.facebook.com/apps](https://developers.facebook.com/apps) → Create App → Business type.

### 2 — Add Facebook Login
Add product → Facebook Login → Web. Under **Valid OAuth Redirect URIs** add your GitHub Pages URL:
`https://YOUR-USERNAME.github.io/kajgod-report-generator/`

### 3 — Request permissions
`pages_show_list`, `read_insights`, `pages_read_engagement`, `instagram_basic`, `instagram_manage_insights`

> In Development Mode these work immediately for the app admin. For client use, submit for Meta App Review (free, ~5 business days).

### 4 — Deploy & use
Push to GitHub, enable Pages (Settings → Pages → main → root). Open the URL, paste your App ID, log in, select page + month, generate.

---

## 📁 Structure

```
kajgod-report-generator/
├── index.html   # Full application — single self-contained file
├── README.md
└── .gitignore
```

---

## 🔒 Privacy

All API calls go directly from the browser to Meta's servers. Nothing is stored or sent to any third party. Read-only permissions only.

---

## Push to GitHub

```bash
cd kajgod-report-generator
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/kajgod-report-generator.git
git push -u origin main
```

Then enable GitHub Pages: Settings → Pages → main branch → root.

---

© kajgod.agency — All rights reserved.
