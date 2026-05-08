# Tim's Inspiring Home Dashboard
**Personal Dashboard · GitHub Pages**

A personal homepage with a spiritual aesthetic — star field background, animated cross, live weather, daily Bible verse, and organized quick-access links.

---

## ✅ Improvements Over AI Studio Version

| Issue | Fix |
|---|---|
| Intermittent failures / cold starts | Pure static HTML — no server, no build step |
| Gemini API key exposed in frontend | Removed — verse now uses Claude API |
| Static weather display | Live real-time weather via Open-Meteo (no key needed) |
| `motion/react` import error | React/Vite stack removed entirely |
| Thin link sections | Expanded to 8 categories with 7–9 links each |

---

## 🚀 Deploy to GitHub Pages

1. Go to [github.com/new](https://github.com/new) → create `tim-home-dashboard` (Private)
2. Click **Add file → Upload files** → drag in `index.html` and `.github/` folder
3. Go to **Settings → Pages → Source → GitHub Actions**
4. Done — live at `https://YOUR_USERNAME.github.io/tim-home-dashboard/`

---

## 🔧 Customizing Links

Edit the `CARDS` array inside `index.html` (around line 280). Each entry:

```javascript
{
  title: 'Category Name',
  icon: `<svg>...</svg>`,
  links: [
    { name: 'Site Name', url: 'https://example.com' },
  ]
}
```

Push to `main` → auto-deploys in ~30 seconds.

---

## 📁 Structure

```
tim-home-dashboard/
├── index.html       ← Everything is here
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```
