# CLAUDE.md - Project Instructions

## Overview
This is a GitHub Pages site at https://manabuozato.github.io/
It serves as an index of test pages, experiments, and small web projects.

## Project Structure
```
manabuozato.github.io/
├── index.html          ← Top page with card-style links to all pages
├── hello/
│   └── index.html      ← Example test page
├── new-page/
│   └── index.html      ← Each page lives in its own folder
└── CLAUDE.md           ← This file
```

## How to Add a New Page

### 1. Create folder and HTML
- Create a new folder with a short, kebab-case name (e.g., `cire-lp`, `manga-viewer`)
- Place `index.html` inside it
- Include a `<a href="../">← Back</a>` link somewhere on the page

### 2. Update the top page index.html
Add a card entry inside `<body>`, after the existing cards:

```html
<a class="card" href="./folder-name/">
  <div class="card-title">Page Title</div>
  <div class="card-desc">Short description</div>
  <div class="card-date">YYYY-MM-DD</div>
</a>
```

Cards should be in reverse chronological order (newest first, after the subtitle).

### 3. Git push
```bash
git add .
git commit -m "add: short description"
git push
```

## Style Notes
- Top page tone: dry British humour, understated
- Pages themselves: whatever style suits the content
- Keep things simple and lightweight, minimal dependencies

## Common Tasks
- "新しいページを作って公開して" → steps 1-3 above
- "一覧を更新して" → step 2 only
- "このHTMLを公開して" → copy provided file into new folder, then steps 2-3
