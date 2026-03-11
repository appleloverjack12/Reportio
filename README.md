# 📊 Meta Report Generator — kajgod.agency

A fully client-side report generator for creating branded monthly social media reports from Meta Business Suite exports.

## ✨ Features

- **Multi-platform** — Facebook, Instagram, LinkedIn
- **Drag & drop uploads** — reads `.xlsx` / `.csv` exports directly from Meta Business Suite
- **Branded PDF output** — matches kajgod.agency visual identity
- **3-step wizard** — configure → upload → preview & export
- **Zero backend** — runs entirely in the browser, no server needed
- **Customisable** — client name, period, brand colours, platforms, custom notes

## 🚀 Usage

### Option 1 — Open locally
Just open `index.html` in any modern browser. No installation needed.

### Option 2 — Host on GitHub Pages
1. Fork this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Access at `https://your-username.github.io/kajgod-report-generator`

## 📁 File Structure

```
kajgod-report-generator/
├── index.html          # Main app (single-file, self-contained)
├── README.md           # This file
├── .gitignore          # Git ignore rules
└── sample-data/        # Example .xlsx files for testing
    ├── sample_views.xlsx
    ├── sample_reach.xlsx
    └── sample_interactions.xlsx
```

## 📤 Supported Export Files

Upload these directly from Meta Business Suite:

| File | Metric |
|------|--------|
| `Views.xlsx` | Page / post views |
| `Reach.xlsx` | Organic + sponsored reach |
| `Interactions.xlsx` | Reactions, comments, shares |
| `Follows.xlsx` | New followers (organic + sponsored) |
| `Link_clicks.xlsx` | Link click data |
| `Viewers.xlsx` | Unique visitors / viewers |
| `Audience_csv.xlsx` | Audience demographics |
| `Top_content_formats.xlsx` | Top performing content types |

> All files are optional — the generator falls back to sample data for any missing file.

## 🛠 Tech Stack

- Vanilla HTML/CSS/JS (no framework)
- [SheetJS (xlsx)](https://sheetjs.com/) — Excel file parsing
- [Chart.js](https://www.chartjs.org/) — Chart rendering
- [jsPDF](https://github.com/parallax/jsPDF) — PDF export
- [Google Fonts](https://fonts.google.com/) — Syne + DM Sans

## 🔒 Privacy

All data processing happens **locally in the browser**. No files or data are ever uploaded to any server.

## 📄 License

© kajgod.agency — All rights reserved.
