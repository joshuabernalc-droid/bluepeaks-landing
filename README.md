# Blue Peaks Innovations — Landing Page

Official landing page for [bluepeaks.io](https://bluepeaks.io).

## Stack

- HTML5 + CSS3 + Vanilla JS — no frameworks, no build step
- Single `index.html` — fully self-contained
- Deployed via GitHub Pages + GitHub Actions

## Structure

```
bluepeaks-landing/
├── index.html              # Landing page (EN/ES/FR/DE/ZH/JA/TH)
├── assets/
│   ├── logo.png            # Blue Peaks Innovations logo
│   └── favicon.ico
├── design-system/
│   ├── index.html          # Design system documentation
│   └── tokens.css          # CSS design tokens (OKLCH)
└── .github/
    └── workflows/
        └── deploy.yml      # Auto-deploy on push to main
```

## Features

- **7 languages**: English, Spanish, French, German, Chinese, Japanese, Thai
- **7 currencies**: USD, CAD, EUR, MXN, JPY, THB, CNY (auto-switches with language)
- **11 sections**: Hero, Trust Bar, Services, VIA Connect deep dive, AI Studio, AI Governance, Metrics, Pricing, Pilot CTA, Footer
- **SOC 2 Type II** compliance badge and security feature list
- **Design System**: full token library for use across all Blue Peaks products
- Responsive: mobile, tablet, desktop
- Count-up animations on scroll
- Sticky nav (transparent → solid)

## Local Development

Open `index.html` directly in your browser. No server needed.

## Deploy

Every push to `main` triggers a GitHub Actions workflow that deploys to GitHub Pages automatically.

## Custom Domain

Add a `CNAME` file with `bluepeaks.io` and configure your DNS:

```
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
CNAME www   bluepeaks-io.github.io
```

## Design System

The design system at `design-system/index.html` documents all color tokens, typography, spacing, components, and motion guidelines for use across VIA Connect, AI Studio, and AI Governance products.

---

© 2026 Blue Peaks Innovations Inc. · Federally incorporated in Canada
