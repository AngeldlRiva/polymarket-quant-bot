# Polymarket Quant Bot

Quant research and execution framework for detecting inefficiencies and potential arbitrage opportunities in Polymarket.

## Project Goals

- Collect live market data from Polymarket
- Parse and store market snapshots
- Detect binary and cross-market arbitrage opportunities
- Model liquidity, slippage, and execution constraints
- Backtest opportunity quality over time
- Build toward paper trading and live execution

## Roadmap

### Phase 0 — Project Setup
- Clean repo structure
- Config management
- Logging and reproducibility

### Phase 1 — Market Data Ingestion
- Fetch active markets
- Filter binary markets
- Retrieve YES/NO token IDs
- Save raw market snapshots

### Phase 2 — Arbitrage Scanner
- Compute gross arbitrage opportunities
- Rank signals by implied edge

### Phase 3 — Liquidity-Aware Execution
- Estimate executable size
- Incorporate order book depth and slippage

### Phase 4 — Historical Storage
- Save snapshots to SQLite
- Build research dataset

### Phase 5 — Analytics and Backtesting
- Analyze opportunity frequency and duration
- Simulate net profitability

### Phase 6 — Paper Trading
- Run live signal monitoring
- Simulate execution in real time

### Phase 7 — Live Trading
- Add execution and risk controls
- Deploy guarded real-money trading

## Tech Stack

- Python
- Requests / HTTPX
- Pandas
- SQLite
- Jupyter
- Matplotlib

## Disclaimer

This project is for quantitative research and educational purposes. Apparent arbitrage opportunities may disappear after fees, slippage, latency, and liquidity constraints.
