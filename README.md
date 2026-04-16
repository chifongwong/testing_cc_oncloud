# TSLA Price Dashboard

A single-page web app that displays a live Tesla (TSLA) stock price dashboard.

## Features

- **Live price** — current TSLA price with daily change ($ and %) color-coded green/red
- **Market status** — shows OPEN or CLOSED
- **Key metrics** — Market Cap, Open, Prev Close, Volume, Avg Volume, P/E Ratio, 52W High, 52W Low
- **Interactive price chart** — Chart.js line chart with range selector: 1D / 5D / 1M / 3M / 1Y
- **Auto-refresh** — data refreshes every 30 seconds
- **Error handling** — loading spinner, error banner with retry button

## Usage

Just open `index.html` in any modern browser. No build step, no dependencies to install.

## Data Source

Data is fetched from the [Yahoo Finance](https://finance.yahoo.com) unofficial API. Requests are routed through [corsproxy.io](https://corsproxy.io) as a CORS fallback when direct browser requests are blocked.

> For informational purposes only. Not financial advice.

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- [Chart.js 4](https://www.chartjs.org/) (via CDN)
