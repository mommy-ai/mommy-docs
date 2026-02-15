# Architecture Overview

```
┌──────────────┐     ┌──────────────┐     ┌─────────────┐
│   Twitter /   │────▶│  MOMMY Core  │────▶│  LLM API    │
│   Telegram    │     │  (Python)    │     │  (DeepSeek) │
└──────────────┘     │              │     └─────────────┘
                     │  ┌─────────┐ │
                     │  │ Market  │─┼────▶ CoinGecko API
                     │  │ Advisor │ │
                     │  └─────────┘ │
                     └──────────────┘
```

## Components

- **MOMMY Engine** — Core chat logic with personality system prompt and conversation memory
- **Market Advisor** — Fetches real-time price data and wraps it in motherly advice
- **Config** — Environment-based configuration for API keys and model settings
