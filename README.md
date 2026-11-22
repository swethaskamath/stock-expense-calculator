# Stock Expense Calculator (India)

A single-page, responsive calculator for the total cost of buying and selling stocks on NSE/BSE.

**Live app:** https://swethaskamath.github.io/stock-expense-calculator/

## What it covers

- Segments: Equity Delivery, Equity Intraday, Futures, Options
- Exchanges: NSE, BSE
- Charges: brokerage (editable), STT, exchange transaction charges, SEBI turnover fee, GST, stamp duty, DP charges
- Output: total charges, gross and net P&L, breakeven move per unit, charges as % of turnover

## Rates used (as of Nov 2026)

| Charge | Delivery | Intraday | Futures | Options |
|---|---|---|---|---|
| STT | 0.1% buy & sell | 0.025% sell | 0.05% sell | 0.15% sell (premium) |
| Txn (NSE) | 0.00307% | 0.00307% | 0.00183% | 0.03553% (premium) |
| Txn (BSE) | 0.00375% | 0.00375% | 0 | 0.0325% (premium) |
| Stamp duty (buy) | 0.015% | 0.003% | 0.002% | 0.003% |
| SEBI fee | ₹10 / crore | ₹10 / crore | ₹10 / crore | ₹10 / crore |
| GST | 18% on brokerage + txn + SEBI | same | same | same |

F&O STT rates reflect the Budget 2026–27 change effective 1 April 2026.

Not modelled: NSE IPFT (₹0.01/crore), STT on exercised options, call-and-trade and auto square-off fees. Figures are estimates; your contract note is final.

## Updating rates

All statutory rates live in the `RATES` object near the bottom of `index.html`. Edit them there when rules change.

## Run locally

Open `index.html` in any browser. No build step, no dependencies.
