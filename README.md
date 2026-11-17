# FRESHCYCLE AI

**Research title:** Stockout-Aware Demand Recovery and Expiry-Constrained Inventory Optimization for Multi-Store Perishable Retail.

FRESHCYCLE AI is a research and simulation platform exploring demand recovery during stockouts, demand forecasting, perishable inventory policies, and multi-store stock transfers.

## Research scope

- Recover latent demand in controlled synthetic stockout experiments.
- Benchmark baseline, LightGBM, XGBoost, and a duration-based hybrid recovery approach.
- Simulate FIFO and FEFO inventory policies with expiry and waste.
- Evaluate a greedy multi-store surplus-to-deficit transfer heuristic.
- Expose research summaries and simulation outputs through a FastAPI API and Streamlit dashboard.

## Reported experimental highlights

- Hybrid demand recovery MAE: 0.152076 versus baseline MAE: 0.165084 on the selected temporal test sample.
- Forecast FEFO fill rate: 91.3482%, compared with fixed FIFO: 84.6395% in the paired inventory simulation.
- Coordinated FEFO transfer simulation contribution gain: 455.5958 scenario credits (+3.0135%) over independent FEFO in the evaluated network.

These are experimental results from selected samples and simulations, not production or real-retailer financial outcomes.

## Important limitations

- The FreshRetailNet-50K source dataset is from China; this project does not establish Indian-market validation.
- The source dataset's sale_amount is normalized, not actual physical units or currency.
- Batch expiry, physical inventory, disposal, store locations, transport costs, prices, and cost parameters are simulated assumptions.
- Synthetic stockout masking is a controlled experiment, not ground-truth lost demand during real stockouts.
- The transfer policy is a greedy heuristic, not a globally optimal routing solution.
- Results are limited to the evaluated samples and scenarios; independent confirmation is needed.

## Application

The application consists of a FastAPI backend and a Streamlit dashboard. See [docs/APP_SETUP.md](docs/APP_SETUP.md) for local setup instructions and [docs/FRESHCYCLE_AI_RESEARCH_RESULTS.md](docs/FRESHCYCLE_AI_RESEARCH_RESULTS.md) for the research summary.

## Repository upload status

This repository has been initialized. The full source archive is not yet present; only this README has been published so far. The project ZIP still needs to be transferred into the repository.

