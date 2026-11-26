# Sentiment feed

`scores.json` holds one Nasdaq/QQQ sentiment score (0–100) per US trading date.

- **Who writes it:** the daily sentiment task adds each new score around 07:45 ET (20:43 Singapore time).
- **Who reads it:** DyRSI live algorithms (QQQ v1.7.3+, TQQQ v1.8.3+) read it through the `raw.githubusercontent.com` URL.
- **What it contains:** dates and scores only. Nothing about accounts or positions.
- **Format:** `{"updated": "...", "scores": {"YYYY-MM-DD": score, ...}}`

Keep this repo **public**. The algorithm reads the file without logging in.
