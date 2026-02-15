# API Reference

## MommyEngine

### `MommyEngine.chat(user_id: str, message: str) -> str`

Send a message to MOMMY and get a response.

- `user_id` — Unique identifier for conversation tracking
- `message` — User's message text
- Returns: MOMMY's response string

## Market Advisor

### `await get_btc_price() -> dict`

Returns `{"price": float, "change_24h": float}` from CoinGecko.

### `get_mommy_advice(change_24h: float) -> str`

Returns motherly advice based on 24h price change.

### `await market_report() -> str`

Full formatted market report with price + advice.
