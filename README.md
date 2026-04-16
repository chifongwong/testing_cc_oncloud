# TSLA Price Dashboard

A single-page web app that displays a live Tesla (TSLA) stock price dashboard.

## Features

- **Live price** — current TSLA price with daily change ($ and %) color-coded green/red
- **Market status** — shows OPEN or CLOSED
- **Key metrics** — Market Cap, Open, Prev Close, Avg Volume (10D), Day High, P/E Ratio, 52W High, 52W Low
- **Interactive price chart** — Chart.js line chart with range selector: 1D / 5D / 1M / 3M / 1Y
- **Auto-refresh** — data refreshes every 30 seconds
- **Error handling** — loading spinner, error banner with retry button

## Setup

1. Get a free API key from [twelvedata.com/register](https://twelvedata.com/register) (takes under a minute)
2. Open `index.html` in any modern browser — no build step, no dependencies to install
3. Paste your Twelve Data API key when prompted — it's saved to `localStorage` for future visits
4. Use the ⚙ button in the header to update the key at any time

## Data Source

Data is fetched from the [Twelve Data](https://twelvedata.com) API, which provides proper CORS support, real-time quotes, and a free tier of 800 API calls/day. No backend or proxy required.

To stay within the free tier, the price refreshes every 2 minutes and the chart only re-fetches when you switch range.

> For informational purposes only. Not financial advice.

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- [Chart.js 4](https://www.chartjs.org/) (via CDN)
- [Twelve Data API](https://twelvedata.com/docs) (free tier)
