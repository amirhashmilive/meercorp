# MEMORY.md — Meer Corporation Website Project

> **Agentic Memory File** | Created: 2026-06-25 | Last Updated: 2026-06-25
> This file documents the complete state of the Meer Corporation website project for continuity across AI agent sessions.

---

## 📋 Project Overview

| Field | Value |
|-------|-------|
| **Project Name** | Meer Corporation Website |
| **Purpose** | Corporate website for Meer Corporation — serves as the company's primary web presence |
| **Owner** | amirhashmilive |
| **Status** | 🟡 Early Stage — Deployed but structurally underdeveloped |
| **Created** | 2026 |

---

## 🌐 Deployment

| Field | Value |
|-------|-------|
| **Platform** | GitHub Pages |
| **Live URL** | https://amirhashmilive.github.io/meercorp/ |
| **GitHub Repo** | https://github.com/amirhashmilive/meercorp |
| **Branch** | `main` (GitHub Pages served from root of `main` branch) |
| **Deployment Method** | Direct commit to `main` branch; GitHub Pages auto-deploys |

### Deployment Notes
- The site currently serves `index.html` from the root of the `main` branch.
- There is **no** `gh-pages` branch; deployment happens directly from `main`.
- To deploy a new version: update `index.html` locally → commit → push to `main`.

---

## 📁 Current File Structure

```
meercorp/
├── index.html        ← 3.4 MB — ENTIRE React app bundled into a single HTML file
├── LICENSE           ← MIT License (1,068 bytes)
└── README.md         ← Essentially empty (10 bytes — only placeholder text)
```

### ⚠️ Critical Structural Issue
The repository currently contains **only 3 files**. The local project directory (`D:\DRIVE (Ai) Agents\00 Projects\meercorp`) was **empty** at audit time — no source files exist locally. The only artefact is the compiled/bundled `index.html` (3.4 MB) committed directly to GitHub.

This means:
- There is **no source code** locally (no `src/`, `components/`, etc.)
- There is **no `package.json`** or build configuration
- The site cannot currently be rebuilt or modified without starting fresh

---

## 🛠️ Technology Stack

| Layer | Technology | Notes |
|-------|-----------|-------|
| **Framework** | React 19.2.3 | Confirmed via bundled source |
| **Build Tool** | Vite | Inferred from bundle structure and `modulepreload` polyfill pattern |
| **Language** | JavaScript (JSX) | No TypeScript detected |
| **Styling** | Unknown (bundled/minified) | Likely CSS Modules or vanilla CSS |
| **Routing** | Unknown | Likely React Router (SPA) |
| **Deployment** | GitHub Pages | Static HTML serving |
| **Bundle Strategy** | All-in-one `index.html` | ⚠️ 3.4 MB single file — no asset splitting |

---

## 🎨 Design Decisions (Observed from Live Site)

Based on what was built and deployed:

1. **Single-Page Application (SPA)** — The entire app is a React SPA rendered client-side.
2. **Single bundle file** — All JS, CSS, and HTML packed into one `index.html`. This is an anti-pattern for production (no code splitting, no caching benefits).
3. **Title set to "Meer Corporation"** — Confirmed in `<title>` tag.
4. **No favicon** — No custom favicon observed.
5. **No meta description** — SEO is essentially non-existent.

> **Note:** Because the site uses client-side React rendering and the HTML is minified/bundled, the exact visual content (sections, colors, layout) could not be fully determined through static analysis alone. A browser-based visual audit would be needed for complete design documentation.

---

## ❌ What's Missing / Gaps Identified

### Critical
- [ ] **No source code locally** — The `D:\DRIVE (Ai) Agents\00 Projects\meercorp` folder was empty. Source must be recreated or recovered from the bundle.
- [ ] **No `package.json`** — Cannot install dependencies or run dev server.
- [ ] **No build pipeline** — No `vite.config.js` or equivalent. Cannot rebuild from source.
- [ ] **3.4 MB single-file bundle** — Extremely heavy for a static site; no asset splitting.

### SEO & Meta
- [ ] No `<meta name="description">` tag
- [ ] No Open Graph tags (`og:title`, `og:image`, etc.)
- [ ] No favicon / `apple-touch-icon`
- [ ] No `sitemap.xml`
- [ ] No `robots.txt`

### Content
- [ ] README.md is empty (10 bytes)
- [ ] No `404.html` page (GitHub Pages SPA routing will break on direct URL access)
- [ ] Contact form backend (if any) — status unknown

### Dev Experience
- [ ] No `.gitignore`
- [ ] No CI/CD pipeline
- [ ] No linting or formatting config

---

## 🗺️ Roadmap / Future Plans

### Phase 1 — Foundation Recovery (Immediate)
1. **Recreate the React + Vite project structure** locally in `D:\DRIVE (Ai) Agents\00 Projects\meercorp`
2. Set up `package.json`, `vite.config.js`, `.gitignore`
3. Implement proper build pipeline with asset splitting (CSS, JS chunks)
4. Add `404.html` for SPA routing on GitHub Pages

### Phase 2 — Content & SEO
1. Populate all pages with real Meer Corporation content
2. Add meta tags, Open Graph, Twitter Card tags
3. Add favicon and app icons
4. Create `sitemap.xml` and `robots.txt`
5. Fill out `README.md` with project description

### Phase 3 — Design Enhancement
1. Implement modern design system (dark mode, brand colors, typography)
2. Add animations and micro-interactions
3. Ensure full responsiveness across all breakpoints
4. Optimize images and assets

### Phase 4 — Advanced Features
1. Contact form with backend (EmailJS, Formspree, or serverless function)
2. Analytics integration (Google Analytics / Plausible)
3. Performance audit (Lighthouse score target: 90+)
4. Accessibility audit (WCAG 2.1 AA compliance)

---

## 📝 Session Log

| Date | Session Summary |
|------|----------------|
| 2026-06-25 | Initial audit performed. Local directory found empty. Repository contains only `index.html` (3.4 MB bundled React app), `LICENSE`, and near-empty `README.md`. MEMORY.md created. |

---

## 🔗 Key Links

- **Live Site:** https://amirhashmilive.github.io/meercorp/
- **GitHub Repo:** https://github.com/amirhashmilive/meercorp
- **Local Path:** `D:\DRIVE (Ai) Agents\00 Projects\meercorp`

---

*Update this file at the start of every new AI agent session to reflect the current state of the project.*
