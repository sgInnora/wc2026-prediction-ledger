# World Cup 2026 — Receipt-Verified AI Prediction Ledger

Every pre-kickoff AI forecast for FIFA World Cup 2026 published by [GoalPulse](https://goalpulse.io), locked in immutable snapshots with sha256 receipts **before kickoff** and scored against official results. Misses included — nothing hidden.

**Live source (updates hourly through the final):** https://goalpulse.io/open-data
**Human-readable track record & calibration:** https://goalpulse.io/ai-track-record
**Final-tournament scorecard (auto-freezes after the final):** https://goalpulse.io/wc2026-verdict

## What's here
- `prediction-ledger.json` — every scored forecast: W/D/L probabilities, actual result, per-row multiclass Brier, calibration buckets, and baselines (model vs de-vig market closing consensus vs uniform 1/3).
- `prediction-ledger.csv` — same rows, flat.
- `knockout-simulation.json` — exact bracket-DP championship probabilities from the current shadow model.

## Honesty notes
- Forecasts are from an editorial shadow model (calibrated Elo). On the joined rows the **market closing consensus still beats the model** (Brier ≈0.446 vs ≈0.499) — we publish the comparison anyway; that's the point.
- Draws in knockout propagation are split proportionally to 90-minute win probabilities (shootout proxy).
- Not betting odds. Not betting advice.

## License & citation
**CC BY 4.0** (see `LICENSE`): free to use, share and adapt — credit **GoalPulse (goalpulse.io)** and link to https://goalpulse.io/open-data. A machine-readable `CITATION.cff` is included; GitHub's "Cite this repository" button works out of the box.

## Projects using this data
Using the ledger in a notebook, article, model eval or app? **Open a PR adding yourself here** — we list every project.

- *(your project here)*

*Snapshot in this repo: 2026-07-15 (91 scored matches, through the semi-finals). For the freshest data, always pull the live endpoints above.*
