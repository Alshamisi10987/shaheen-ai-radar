# Shaheen | AI Adoption and Opportunity Radar

Shaheen (شاهين) is a single-page web dashboard designed to identify, assess, and prioritize AI adoption and sales opportunities across the UAE market.

The dashboard organizes companies, government entities, authorities, free zones, investors, and strategic partners based on their AI adoption level, buying intent, and product fit. It then highlights the most promising opportunities and suggests the next best action for engagement.

## Live Demo

[Open Shaheen AI Radar](https://alshamisi10987.github.io/shaheen-ai-radar/)

## Key Features

- **Opportunity Leaderboard** — ranks prospects using adoption, intent, and product-fit scores
- **Advanced Search and Filters** — filter by emirate, sector, entity type, product, and score range
- **KPI Overview** — displays market size, high-priority leads, product fit, and active signals
- **Live Signal Feed** — pulls and merges real news signals from free external sources
- **Live Data Status Chip** — clearly shows feed state as `LIVE`, `LIMITED`, or `FALLBACK`
- **In-Page Settings Modal** — configure API keys and query directly from the dashboard (no browser prompts)
- **Real-Only / Fallback Control** — choose strict live-only mode or allow archive fallback for higher continuity
- **Prospect Profiles** — provides detailed entity information, product-fit insights, and suggested outreach messages
- **Export Tools** — exports filtered results, prospect profiles, and sales-ready metrics
- **Product Radar Chart** — visualizes adoption and product-fit performance across different solutions

## Technology Stack

Shaheen is built as a lightweight, self-contained web application with no build process required.

- HTML5
- CSS3
- Vanilla JavaScript
- Google Fonts
- Inter and Space Grotesk typefaces

## Getting Started

No installation is required.

### Option 1: Open Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/Alshamisi10987/shaheen-ai-radar.git
   ```

2. Open the project folder.

3. Open `index.html` in your browser.

### Configure Live News (Recommended)

News is fetched directly in your browser from free, keyless sources (GDELT and Google News RSS) — no backend or server setup required.

1. Click **Settings** in the top-right of the dashboard.
2. (Optional) Add a **GNews API key** (free tier) for broader coverage.
3. (Optional) Add a **NewsData.io API key** for broader coverage.
4. Set your preferred query (example: `UAE AI OR artificial intelligence`).
5. Choose whether to enable archive fallback when live APIs are limited.

Notes:
- API keys are stored locally in your browser (`localStorage`) and are never sent anywhere except directly to the provider you configured.
- Free API tiers may rate-limit requests, which can temporarily show status as `LIMITED`.

### Option 2: Use the Live Version

Access the deployed project through GitHub Pages:

[https://alshamisi10987.github.io/shaheen-ai-radar/](https://alshamisi10987.github.io/shaheen-ai-radar/)

## Project Structure

```text
shaheen-ai-radar/
├── index.html
└── README.md
```

## Live Data Behavior

- `LIVE`: External live sources are responding and current signals are being refreshed.
- `LIMITED`: One or more live providers are temporarily constrained (for example rate limits or query rejection).
- `FALLBACK`: Live sources are unavailable and archive fallback is being used (if enabled).

This status appears in the header so users can quickly understand feed quality and freshness.

## Latest Website Updates

- Replaced prompt-based settings flow with a dedicated in-page settings modal.
- Added optional multi-source news ingestion to improve resilience.
- Added query cleanup and request hardening for free-tier API reliability.
- Added visible live status labeling (`LIVE` / `LIMITED` / `FALLBACK`).

## Purpose

Shaheen was created to support the identification and prioritization of AI adoption opportunities across the UAE market. It provides a clear, structured view of potential prospects and helps decision-makers focus on high-value opportunities.

## Deployment

The project is deployed using GitHub Pages from the `main` branch and the repository root folder.

## License

This project is currently provided for demonstration and portfolio purposes.