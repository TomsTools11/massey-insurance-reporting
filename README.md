# Massey Insurance — Performance Reports

Static reporting site for the Massey Insurance account, plus four performance
reports for the July 8–31, 2026 reporting period.
Built as plain HTML/CSS (no build step) and deployed on Vercel.

## Structure

```
index.html                                  Report hub (landing page)
reports/geographic-performance.html         Report 01 — Geographic Performance
reports/inbound-call-performance.html       Report 02 — Inbound Call Performance
reports/auto-campaign-performance.html      Report 03 — PA Auto Campaign
reports/home-campaign-performance.html      Report 04 — PA Home Campaign
assets/                                      GOAL brand marks (PNG)
vercel.json                                  Static deployment config
```

## Deployment

This is a zero-config static site. On Vercel:

1. Import the repository (Framework Preset: **Other** — auto-detected, no build command).
2. Deploy. `index.html` is served at `/`; reports are served at
   `/reports/<name>.html`.

Every push to `main` triggers a production deploy once the Vercel project is linked.

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.
