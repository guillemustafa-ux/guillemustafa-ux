### Guillermo Mustafa · Trading systems engineer

Pine Script v6 indicators and strategies, backtest audits in Python, broker execution on demo and paper accounts. Every repo below is a runnable proof: it states a claim and shows how to check it.

#### TradingView scripts (open source)

| Script | What it checks | Code |
|---|---|---|
| [RSI Divergence vs Random Bars](https://www.tradingview.com/script/LxAhwOxK-RSI-Divergence-vs-Random-Bars-Does-It-Call-the-Turn/) | Measures whether regular RSI divergences call the turn more often than the same swing without divergence and than random bars | [rsi-divergence-vs-random](https://github.com/guillemustafa-ux/rsi-divergence-vs-random) |
| [Fibonacci vs Random Ratios](https://www.tradingview.com/script/MV9tTaED-Fibonacci-vs-Random-Ratios-Where-Pullbacks-Actually-Stop/) | Tests whether pullbacks stop near the Fibonacci levels more often than near random ratios with the same tolerance, and how many random sets do as well | [fibonacci-vs-random](https://github.com/guillemustafa-ux/fibonacci-vs-random) |
| [Heikin Ashi Fill Gap](https://www.tradingview.com/script/oTHxF7ou-Heikin-Ashi-Fill-Gap-What-a-Backtest-Gains-at-HA-Prices/) | Measures the gap between Heikin Ashi and real prices, and what the same signal gains when a backtest fills at HA prices | [heikin-ashi-fill-gap](https://github.com/guillemustafa-ux/heikin-ashi-fill-gap) |
| [Data Age](https://www.tradingview.com/script/txAVsq9Y-Data-Age-How-Old-Is-the-Value-request-security-Returns/) | Measures how old the value `request.security` returns is for up to three symbols, and counts the bars where it was carried forward | [request-data-age](https://github.com/guillemustafa-ux/request-data-age) |
| [Session DST Audit](https://www.tradingview.com/script/EMa1CDGm-Session-DST-Audit-Does-a-Fixed-Offset-Session-Drift/) | Checks one session string in a DST-aware zone and a fixed offset, and counts the bars each one misses or adds | [session-dst-audit](https://github.com/guillemustafa-ux/session-dst-audit) |
| [Intrabar Ambiguity](https://www.tradingview.com/script/QXyp6oKQ-Intrabar-Ambiguity-Which-Hit-First-Stop-or-Target/) | Finds bars where stop and target both fit in one range and settles them with lower-timeframe data | [intrabar-ambiguity](https://github.com/guillemustafa-ux/intrabar-ambiguity) |
| [Repaint Auditor](https://www.tradingview.com/script/7USFvRmd-Repaint-Auditor-Live-Flicker-Counter-and-request-security-A-B/) | Counts intrabar repaints and ghost signals live, and A/B tests three `request.security` forms | [repaint-auditor](https://github.com/guillemustafa-ux/repaint-auditor) |
| [Cost Ladder](https://www.tradingview.com/script/kQRPTxtz-Cost-Ladder-Does-a-Signal-Survive-0x-1x-and-2x-Costs/) | Re-prices the same trades at 0x, 1x and 2x costs, with a 95% CI and the break-even cost | [cost-ladder](https://github.com/guillemustafa-ux/cost-ladder) |
| [Seasonality vs Shuffled Calendar](https://www.tradingview.com/script/5RcwXxp7-Seasonality-vs-Shuffled-Calendar-Is-the-Best-Month-Real/) | Tests the best month or weekday against a shuffled calendar | [seasonality-shuffle](https://github.com/guillemustafa-ux/seasonality-shuffle) |
| [Candlestick Patterns vs Baseline](https://www.tradingview.com/script/fGFxqicu-Candlestick-Patterns-vs-Baseline-Forward-Returns-95-CI/) | Six candlestick patterns against an all-bars baseline, with a 95% CI | [candlestick-base-rates](https://github.com/guillemustafa-ux/candlestick-base-rates) |
| [Liquidity Sweep, MSS and FVG with Look-ahead A/B](https://www.tradingview.com/script/2pqi4yFB-Liquidity-Sweep-MSS-and-FVG-Entry-Model-with-Look-ahead-A-B/) | ICT entry model as a `strategy()`, with a built-in look-ahead demo | [ict-sweep-mss-fvg](https://github.com/guillemustafa-ux/ict-sweep-mss-fvg) |
| [GEX Levels with OI Age Check](https://www.tradingview.com/script/uKwF557w-GEX-Levels-from-a-Level-String-with-OI-Age-Check/) | Gamma-exposure levels with a freshness verdict on the open interest | [gex-levels-proof](https://github.com/guillemustafa-ux/gex-levels-proof) |

All scripts on TradingView: [GuilleMustafa](https://www.tradingview.com/u/GuilleMustafa/)

#### Backtests and execution

- [backtest-audit-proof](https://github.com/guillemustafa-ux/backtest-audit-proof): a naive backtest finds an edge in data with none; the audit takes it apart artifact by artifact.
- [backtest-to-production-proof](https://github.com/guillemustafa-ux/backtest-to-production-proof): one strategy walked from a naive backtest to an offline order path, and how much of the claim survives each stage.
- [bidask-execution-proof](https://github.com/guillemustafa-ux/bidask-execution-proof): a 1-second backtest re-executed on real bid/ask and book data, removing one fill assumption at a time.
- [ibkr-reconnect-proof](https://github.com/guillemustafa-ux/ibkr-reconnect-proof): idempotent order handling and state resync against the IBKR TWS API, verifiable without an account.
- [tradingview-mcp-proof](https://github.com/guillemustafa-ux/tradingview-mcp-proof): an MCP server that refuses to hand stale TradingView data to an LLM as live prices.

#### Work with me

Custom Pine Script, backtest audits and broker integrations: [Upwork profile](https://www.upwork.com/freelancers/~01fa3c5136b53674c8)
