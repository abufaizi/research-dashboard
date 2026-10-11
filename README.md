# Research Dashboard

Static research dashboard. There is no build step.

Deploy with Cloudflare Pages:

- Build command: empty
- Output directory: `/`

## Daily Clips tab

The Daily Clips tab loads `data/clips/index.json` and the daily digests
`data/clips/YYYY-MM-DD.json`. The daily-clips pipeline writes these files when
`DASHBOARD_CLIPS_DIR` points to this folder. Commit and push them to publish.
Until the folder has data, the tab shows a "No clip digests published yet" message.
