# TSLA Price Dashboard

A single-page web app that displays a live Tesla (TSLA) stock price dashboard.

## Features

- **Live price** — current TSLA price with daily change ($ and %) color-coded green/red
- **Key metrics** — Open, Prev Close, Day High, Day Low
- **Live chart** — accumulates real price data points every 30 seconds
- **Auto-refresh** — data refreshes every 30 seconds
- **Error handling** — loading spinner, error banner with retry button

## Setup

1. Get a free API key from [finnhub.io/register](https://finnhub.io/register) (takes under a minute)
2. Open `index.html` in any modern browser — no build step, no dependencies to install
3. Paste your Finnhub API token when prompted — saved to `localStorage` for future visits
4. Use the ⚙ button in the header to update the key at any time

## Data Source

Uses only the Finnhub [`/quote`](https://finnhub.io/docs/api/quote) endpoint — the one endpoint that is genuinely free with no tier restrictions. No proxy required.

> For informational purposes only. Not financial advice.

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- [Chart.js 4](https://www.chartjs.org/) (via CDN)
- [Finnhub API](https://finnhub.io/docs/api) — `/quote` endpoint (free tier)

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
