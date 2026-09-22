# Cheer Gym Tryout Evaluator

Standalone local reconstruction of the Bolt.new cheer placement engine.

## Run locally

From this directory, start a static server:

```sh
python3 -m http.server 4173
```

Open `http://127.0.0.1:4173/` in a browser.

The app is contained in `index.html` and supports roster paste, CSV/TSV and PDF upload, USASF 2025-2026 team selection, automated sorting, compliance alerts, and manual placement overrides. `cheer_tryout_verified_v4.html` is preserved as the alternate standalone export found alongside the source material.