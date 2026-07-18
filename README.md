# Pinescript Contra Pivot SuperTrend Fade Strategy

Pine Script v6 fade strategy that trades against exhaustion moves into the Pivot Point SuperTrend band: touch/reversal/both triggers, pyramiding, and trailing management.

## Features

- Contra / mean-reversion logic that fades stretched moves into the Pivot Point SuperTrend band (SELL when price stretches up into the band, BUY when it stretches down).
- Three selectable signal triggers: `Touch` (price tags the band), `Reversal` (SuperTrend regime flips through the band), or `Both`.
- Pyramiding into the profit direction with configurable step type — Points, Percent, or ATR — and a max add count.
- Confluence filters: ORB (opening-range) outside filter, ADX minimum, optional ATR floor, and an optional EMA-side filter.
- Target, fixed stop-loss, and trailing-stop management, each toggleable in Points or Percent.
- Re-entry-safe state handling: pyramid/trail anchors are re-seeded from the real average fill on the bar a position opens and cleared while flat, so nothing leaks across trades.
- Built-in diagnostics table and lower-pane plots (Pivot SuperTrend, EMA, ORB levels, ADX, ATR, entry markers).

## Stack

- Pine Script v6 (TradingView strategy script), single file `contra-pivot-supertrend-v6.pine`.

## Getting started

1. Open the [TradingView](https://www.tradingview.com) Pine Editor.
2. Create a new script and paste the contents of `contra-pivot-supertrend-v6.pine`.
3. Click "Add to chart" and open the Strategy Tester to backtest.
4. Tune inputs (signal trigger, pivot/ATR settings, filters, pyramiding, target/SL/trailing) to your instrument and timeframe.

## Notes

Trading automation is infrastructure, not financial advice. No profit guarantees. Test in dry-run/paper before live.

## Author

Built by [Jayadev Rana](https://jayadevrana.in) — @bluealgocapital · [YouTube](https://www.youtube.com/@jayadevrana3657) · [GitHub](https://github.com/jayadevrana)
