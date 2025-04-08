# Option-Markets-Delta-Gamma
Analysis of a stock or ETFs option market using weighted deltas & gammas across expirations and strikes.

This is a rough cut — messy code, but the core logic works and the insights are solid (or getting there).

Scrapes SPY option chain and calculates:
  Weighted Delta = Open Interest × Delta
  Weighted Gamma = Open Interest × Gamma

These values are grouped by strike and expiration to visualize where the market might be long or short delta/gamma, and how that may affect price behavior.

Key Concepts:
  Dealer gamma/delta exposure can push or dampen volatility
  Large shifts around expiry often coincide with directional bias
  Understanding where gamma flips can help anticipate market behavior

Big issue is data quality coming from YFinance - beggers can't be choosers.

Goals:
  Convert data to real time
  Move from NGrok tunnel to live website
  Add Vega and Charm measures
