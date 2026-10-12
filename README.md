### Hi, I'm Leigh

Data science student focused on **data engineering** and **quantitative
research**. I like work where the hard part is making the numbers
trustworthy: finding the duplicated rows, the restated fundamentals and the
overfit backtest before they reach a conclusion.

#### Featured: [filing-signals](https://github.com/Samarty-1/filing-signals) · [live explorer](https://samarty-1.github.io/filing-signals/)

SEC 10-K text, end to end, in **Python, SQL, Rust and TypeScript**:
- A point-in-time EDGAR warehouse. It found that the API's acceptance time is
  wrong by 4–5 hours for 11.5% of filings.
- A Rust section parser via PyO3, 23× faster than the Python spec and
  identical on all 8,082 documents.
- Three fine-tuned models on one RTX 4070:
  - QLoRA Qwen-1.5B reads revenue out of MD&A at **91% precision**, against
    20% zero-shot.
  - FinBERT and a fine-tuned embedder **lose to TF-IDF**, and the write-up
    says so.
- A pre-registered return test.

#### Products for small businesses

Working software with a demo you can run, a web app, Docker and CI:

| Product | What it does |
|---|---|
| [fairshift](https://github.com/Samarty-1/fairshift) | Staff rostering for cafés and shops with OR-Tools CP-SAT. The rota is legal (Singapore Employment Act defaults), fair and costed in under a second; every gap has a reason; and a sick call is re-planned with minimal changes |
| [payout-recon](https://github.com/Samarty-1/payout-recon) | Reconciles orders, Stripe, GrabFood and foodpanda payouts, and the bank. Finds missing payouts, commission above contract and over-refunds (8/8 planted problems on every synthetic test month), then writes a balanced Xero journal |
| [invoice-intake](https://github.com/Samarty-1/invoice-intake) | Supplier invoices to bookable data on a **local LLM**. Blocks wrong GST, bad totals, duplicates and changed bank details. 100% field accuracy on held-out layouts where hand-written rules scored 0% (synthetic) |
| [countbone](https://github.com/Samarty-1/countbone) | Stock counting from phone video, through to the ERP adjustment and a signed supplier claim |

#### Data engineering & SQL

| Project | What it shows |
|---|---|
| [citibike-warehouse](https://github.com/Samarty-1/citibike-warehouse) | Star schema over 4.3M bike trips. An SCD2 station dimension built by entity resolution through a 2021 ID migration lets growth be measured like-for-like: **+31%, not the naive 2.6×** |
| [nyc-taxi-dbt](https://github.com/Samarty-1/nyc-taxi-dbt) | dbt + DuckDB over 30M taxi records, with schema drift, voided-charge pairs and double-counted surcharges. Includes a placebo-checked diff-in-diff on whether congestion pricing sped up traffic |
| [retail-sql-analytics](https://github.com/Samarty-1/retail-sql-analytics) | Cohorts, RFM and basket lift in plain SQL on 1M transactions. Reconciling raw to model caught **£680k** of double-counted or reversed sales |
| [point-in-time-warehouse](https://github.com/Samarty-1/point-in-time-warehouse) | Bitemporal market-data warehouse: restated fundamentals lift a strategy's Sharpe from **0.17 to 0.27**. My first published figure (0.33 → 0.91) was mostly look-ahead in the measurement, found and corrected in a later audit |

#### Quant research

| Project | What it shows |
|---|---|
| [backtest-overfit-audit](https://github.com/Samarty-1/backtest-overfit-audit) | Deflated Sharpe, PBO and multiple-testing haircuts, pointed at my own strategies (they fail) |
| [cotangent](https://github.com/Samarty-1/cotangent) | Header-only C++20 reverse-mode AD: every Monte Carlo Greek for roughly the cost of one valuation |
| [black-scholes-plus](https://github.com/Samarty-1/black-scholes-plus) | Tested option-pricing library: robust implied vol, American trees, Heston, SVI, with docs and a dashboard |
| [market-signal-dashboard](https://github.com/Samarty-1/market-signal-dashboard) | Live data, walk-forward model, honest out-of-sample backtest and a daily retraining Action |
| [sreit-analytics](https://github.com/Samarty-1/sreit-analytics) | Singapore REIT rate sensitivity, and a valuation signal that fails out of sample |

#### Other

[bot-detection](https://github.com/Samarty-1/bot-detection): adversarial
bot detection on synthetic ticketing traffic ·
[nexus-chess](https://github.com/Samarty-1/nexus-chess): in-browser chess
with Stockfish and P2P play

**Tools:** Python, SQL (DuckDB, dbt), Rust (PyO3), C++20, TypeScript, PyTorch
(QLoRA, PEFT), OR-Tools, FastAPI, Docker, pandas, NumPy/SciPy, Streamlit, GitHub Actions
