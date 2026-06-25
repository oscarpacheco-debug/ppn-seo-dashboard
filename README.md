# papernest Growth SEO Dashboard

Interactive weekly off-page performance dashboard. Reads directly from your Google Sheets Master Data.

## Deploy to GitHub Pages (free, 5 minutes)

1. Create a new **public** repository on GitHub (e.g. `ppn-seo-dashboard`)
2. Upload `index.html` to the root
3. Go to **Settings → Pages → Source** → select `main` branch → Save
4. Your dashboard is live at `https://yourusername.github.io/ppn-seo-dashboard/`

## Connect your Google Sheet

1. Open your Growth SEO Dashboard Google Sheet
2. Click **Share** → change access to **"Anyone with the link can view"**
3. Open the dashboard URL
4. Paste the sheet URL and click **Connect Sheet**

The app reads your `📊 Master Data` tab directly. No API keys, no backend, no cost.

## How it works

- Reads `📊 Master Data` via the Google Sheets public CSV export endpoint
- Filters `Source Flow = SEO/Whale` rows client-side
- Aggregates by Market + Year + Week on the fly
- All computation happens in the browser — nothing is stored

## Filters

- **Market**: Spain / Italy / France
- **Year**: all years present in Master Data
- **Week**: all weeks for the selected market + year, plus "All weeks" for full-year view

## Tabs

- **Overview** — KPIs + best link + BL trend + topic donut + DR distribution + campaign bar
- **Campaigns** — sortable table of all campaigns with BL, RP, Avg DR, New RD
- **Topics** — topic breakdown with bar chart
- **Trend** — week-by-week BL + DR line chart + full weekly table
