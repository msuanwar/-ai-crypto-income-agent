# Codex instructions

- Preserve the paper-only safety boundary. Do not implement real order placement, margin, futures, leverage, withdrawals or live API credentials.
- Use Python 3.11+, type hints, small modules and tests.
- Treat the final kline as potentially incomplete and exclude it from signals.
- Never claim a strategy is profitable. Report assumptions, fees, slippage and drawdown in future backtests.
- Before changing risk logic, add tests for boundary cases.
- Keep secrets out of Git; `.env` is ignored.
- Run `pytest -q` after every change.
- Phase 2 may add historical data ingestion and a backtester, still without live orders.
