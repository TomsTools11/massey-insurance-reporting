# Massey Insurance — Account Hub

Static account hub for the Massey Insurance account, plus two onboarding reports.
Built as plain HTML/CSS (no build step) and deployed on Vercel.

## Structure

```
index.html                                  Account hub (landing page)
reports/campaign-setup-plan.html            Report 01 — Campaign Setup & Plan
reports/going-forward-strategy-process.html Report 02 — Going Forward: Strategy & Process
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
