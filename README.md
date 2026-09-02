# Engineering Program — Campaign Success Tracker (Web)

Self-contained HTML dashboard for the **AKIJ Resource Engineering Program** campaign ROI tracker.

- **Cement (ACCL)** + **Ispat (AIL)** — filter with **Both / Cement / Ispat**.
- Tabs mirror every Excel sheet: **Dashboard · Methodology · Assumptions · Data · Control Market · Analysis · Results · Sources**.
- Only aggregated **results** are published — no DWH credentials or backend.

## Deploy

This is a static site — deploy `index.html` as-is (Vercel "Other" preset, root = `/`).

## Refresh

The file is generated locally by `generate_dashboard.py` (reads the two Excel trackers via Excel COM), then published with `refresh_and_publish.bat`. See the source `v3` folder for the generator and sync scripts.
