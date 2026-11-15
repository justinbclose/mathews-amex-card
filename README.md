# Mathew's Amex Card

A self-contained phone web app that tracks American Express Platinum credits, perks and news.

**Live app:** https://justinbclose.github.io/mathews-amex-card/

## How it works

- Everything lives in one file: `index.html`. No login, no build step, no server.
- Checkmarks and setup progress are saved in each visitor's own browser (`localStorage`), so every phone keeps its own list.
- The News tab, alerts and daily briefing come from one JSON block in `index.html`:
  `<script type="application/json" id="pnews">…</script>`.
  A scheduled Claude task refreshes that block every morning (about 7:45 a.m. Pacific) and pushes to `main`, which redeploys GitHub Pages.

## Add it to an iPhone home screen

1. Open the link above in **Safari**.
2. Tap **Share**, then **Add to Home Screen**, then **Add**.

On Android: Chrome menu, then **Add to Home screen**.
