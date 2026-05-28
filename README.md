# SAYANJALI NEXUS — Founder OS

> Ultra-premium founder portfolio for **Syed Ali Hasan Moosavi**, Founder &amp; Managing Director of **SAYANJALI NEXUS PRIVATE LIMITED**.

A cinematic, AI-inspired static website — built as a self-contained Founder Operating System showcasing the company, flagship products (NexusRank AI, MA Hospital, SYJ Token Ecosystem), R&amp;D and the full technology ecosystem.

---

## ✨ Highlights

- 100% static — HTML5 / CSS3 / vanilla JavaScript. **No build step, no backend.**
- Cinematic dark futuristic UI · glassmorphism · particle network · animated grid · cursor glow · orbit rings
- Animated identity rotator, scroll-reveal sections, animated counters, holographic cards
- Fully responsive (mobile-first, tested 360 → 1920 px)
- Accessibility: semantic HTML, focus states, `prefers-reduced-motion` support, ARIA labels
- Complete SEO + GEO stack: JSON-LD (Person, Organization, WebSite, SoftwareApplication, FAQ), Open Graph, Twitter Cards, canonical URLs, sitemap, robots, manifest
- Optimized for AI search discovery (ChatGPT / Claude / Perplexity / Gemini / Copilot) via rich structured data and machine-readable founder &amp; product entities

---

## 📁 Project Structure

```
portfolio-os/
├── index.html              # Hero command center + all main sections
├── about.html              # Founder profile
├── projects.html           # Case studies
├── ecosystem.html          # Full ecosystem map
├── research.html           # R&D tracks
├── contact.html            # Contact command center
├── css/style.css           # Design system + components
├── js/main.js              # Particles, rotator, reveals, counters
├── assets/
│   ├── icons/favicon.svg
│   ├── images/og-cover.svg
│   └── videos/
├── seo/
│   ├── robots.txt
│   ├── sitemap.xml
│   └── manifest.json
└── README.md
```

> Note: `robots.txt`, `sitemap.xml` and `manifest.json` live inside `/seo/` per the project spec. For GitHub Pages to serve them at the **root URL** (recommended for SEO), copy or symlink them to the repo root. See **Deployment** below.

---

## 🚀 Deployment — GitHub Pages

### Option A — One-click (recommended)

1. Create a new public GitHub repository, e.g. `shalimoosavi.github.io` (user site) or `portfolio` (project site).
2. Upload **all files** from this folder to the repo root.
3. **Copy SEO files to root for proper indexing:**
   ```bash
   cp seo/robots.txt ./robots.txt
   cp seo/sitemap.xml ./sitemap.xml
   cp seo/manifest.json ./manifest.json
   ```
4. In your repo: **Settings → Pages → Source: `Deploy from a branch` → Branch: `main` / `(root)` → Save**.
5. Wait ~30s. Your site is live at `https://<username>.github.io/` (user site) or `https://<username>.github.io/<repo>/` (project site).

### Option B — Git CLI

```bash
git init
git add .
git commit -m "Launch Founder OS"
git branch -M main
git remote add origin https://github.com/SHalimoosavi/<repo>.git
git push -u origin main
```

Then enable Pages in repo Settings (same as Option A step 4).

### Project-site path note

If you deploy as a **project site** (`/<repo>/` subpath), update absolute URLs in:
- `index.html` and each page: `<link rel="canonical">` and `<meta property="og:url">`
- `seo/sitemap.xml` (all `<loc>` entries)
- `seo/robots.txt` (the `Sitemap:` line)

For a **user site** at `https://shalimoosavi.github.io/`, the defaults already match.

---

## 🧪 Local Preview

No build step — just open `index.html` in a browser, or run a tiny static server:

```bash
# Python
python3 -m http.server 8080
# Node
npx serve .
```

Then visit <http://localhost:8080>.

---

## 🎨 Design System

Tokens live in `css/style.css` under `:root`. Key tokens:

| Token | Purpose |
|---|---|
| `--bg`, `--bg-2`, `--panel` | Surfaces |
| `--accent` (cyan), `--accent-2` (violet), `--accent-3` (mint), `--accent-4` (amber) | Accent palette |
| `--grad-1`, `--grad-2`, `--grad-3` | Signature gradients |
| `--font-display` (Space Grotesk), `--font-sans` (Inter), `--font-mono` (JetBrains Mono) | Typography |
| `--radius`, `--glow` | Shape &amp; depth |

All components consume these tokens — change a value, the whole system updates.

---

## 🔍 SEO &amp; GEO

- **Schemas:** Person, Organization, WebSite, SoftwareApplication (×2), FAQPage
- **Per-page meta:** unique title, description, canonical, OG, Twitter
- **AI/GEO-readable entities** for: Syed Ali Hasan Moosavi, SAYANJALI NEXUS, NexusRank AI, MA Hospital, SYJ Token
- Sitemap covers all 6 routes · robots allow-all · manifest for installable PWA shell

---

## 📞 Contact

- WhatsApp: **+91 8008123605**
- Mobile: **+91 6304225807**
- Email: **cto@sayanjalinexus.com** · **founders@syj-token.com** · **shalimoosavi@gmail.com**
- GitHub: <https://github.com/SHalimoosavi>
- LinkedIn: <https://www.linkedin.com/in/syed-ali-hasan-moosavi-237734378/>

---

© SAYANJALI NEXUS PRIVATE LIMITED · Designed &amp; built by Syed Ali Hasan Moosavi
