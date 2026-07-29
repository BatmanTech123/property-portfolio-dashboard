# Property Portfolio Dashboard

A single-file, no-build, no-server dashboard for tracking a portfolio of anything with a value, a category, and a history. Ships with a sample real-estate portfolio; the architecture underneath is domain-agnostic.

**Live demo:** *(your GitHub Pages URL goes here once published)*

## Quick start

1. Open `index.html` in a browser — no install, no build step. That's the whole app.
2. Click **Simulate Market Update** a few times to see history, sparklines, and moving averages populate.
3. Click **Raw Fetch (no JS)** in the top bar to see what a crawler or link preview sees vs. what you see.
4. Explore the **Architecture** tab inside the app for the actual design writeup — public/private data split, why simulation instead of a fake API, how the gamified stats are computed.

## Use it for your own data

- **Quick fork:** edit the `DEFAULT_DATA` object near the top of the `<script>` block in `index.html`.
- **Real separation:** put your data in a private GitHub repo as `data.json` (see `data.json` in this repo for the shape), generate a fine-grained personal access token scoped to just that repo (Contents: read), and paste your username/repo/token into the bar at the top of the dashboard. Your data loads live, your public repo stays generic.

## Stack

Vanilla HTML/CSS/JS. No framework, no npm, no backend. Persistence is `localStorage`. That's a deliberate tradeoff — zero infrastructure, no server costs, works offline except for the optional GitHub connection — not an oversight.

## License

MIT — see `LICENSE`.
