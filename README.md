# APAC Macro Dashboard

Live dashboard tracking macroeconomic indicators across 8 APAC markets:
Singapore, Japan, Australia, South Korea, Indonesia, Philippines, Vietnam, and Malaysia.

## Features

- **FX Rates** — Live EUR exchange rates via ExchangeRate-API + 6-month historical trend (ECB/Frankfurter)
- **Inflation** — CPI annual % from World Bank
- **Interest Rate** — Lending rate % from World Bank
- **GDP Growth** — Annual GDP growth % from World Bank

## Deploy

### Netlify
1. Connect this repo at [app.netlify.com](https://app.netlify.com/) → Add new site → Import from GitHub
2. No build settings needed — it auto-detects

### Vercel
1. Connect this repo at [vercel.com/new](https://vercel.com/new) → Import from GitHub
2. No build settings needed — it auto-detects

## API Keys (both free)

On first visit, the dashboard prompts for two API keys (saved in your browser):

1. **ExchangeRate-API** — [exchangerate-api.com](https://www.exchangerate-api.com/) — for live FX rates
2. **FRED API** — [fred.stlouisfed.org](https://fred.stlouisfed.org/docs/api/api_key.html) — for monthly interest rates

## Data Sources

| Indicator | Source | Frequency |
|-----------|--------|-----------|
| FX Rates (live) | ExchangeRate-API | Daily |
| FX Rates (historical) | ECB via Frankfurter | Daily |
| Interest Rates | FRED (OECD) | Monthly |
| Inflation, GDP | World Bank | Annual |

### Interest Rate Series
| Country | FRED Series | Type |
|---------|------------|------|
| Japan | IRSTCB01JPM156N | Central Bank Rate |
| Australia | IRSTCB01AUM156N | Central Bank Rate |
| South Korea | IRSTCB01KRM156N | Central Bank Rate |
| Indonesia | IRSTCB01IDM156N | Central Bank Rate |
| Singapore | IR3TIB01SGM156N | 3-Month Interbank |
| Philippines | IR3TIB01PHM156N | 3-Month Interbank |
| Vietnam | IR3TIB01VNM156N | 3-Month Interbank |
| Malaysia | IR3TIB01MYM156N | 3-Month Interbank |
