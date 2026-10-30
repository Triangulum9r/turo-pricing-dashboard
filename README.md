# Turo Pricing Dashboard

Static interactive dashboard for Julius's Turo pricing watch (Polestar 4 + Kia EV9).
Published via GitHub Pages from this repo's root. `index.html` renders `data.json`,
which the pricing pipeline re-exports and pushes after each stage run — the page
always shows the latest published snapshot and stamps it "Data as of".

The published data is the MARKET-ONLY view (exporter `--public`): guest-visible
figures any competitor could observe on Turo — frame totals, ranks, trajectories.
Decisions, rationale, lede, coverage notes, and every other strategy artifact are
stripped by an allowlist before export and never enter this repo's data. (Pages
serves a public site even from a private repo, so the repo stays private AND the
data is public-safe.)
