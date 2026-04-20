# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Retail-IQ is a machine learning sales forecasting system for retail time-series data. Uses XGBoost for prediction on Favorita store sales data.

## Setup Commands

```bash
# Create and activate environment
uv venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install package in editable mode
uv pip install -e .

# Run tests (when tests/ exists)
pytest tests/
```

## Architecture

```
src/retail_iq/           # Core Python package
├── config.py             # Path constants (PROJECT_ROOT, DATA_DIR, OUTPUT_DIR, etc.)
├── preprocessing.py      # Data loading, merging, outlier detection
├── features.py           # FastFeatureEngineer class for feature pipeline
└── visualization.py       # Plotting utilities (decomposition, heatmaps, distributions)
```

**Key principle**: Notebooks (`notebooks/eda.ipynb`) are clean drivers only. All logic lives in `src/retail_iq/`.

## Core Modules

### config.py

Path constants using Pathlib. **Always use these for I/O** — never hardcode paths.

- `PROJECT_ROOT`, `DATA_DIR`, `RAW_DATA_DIR`, `PROCESSED_DATA_DIR`
- `OUTPUT_DIR`, `PLOT_DIR`, `MODEL_DIR`, `LOG_DIR`

### preprocessing.py

- `load_raw_data()` — loads train, test, stores, oil, holidays, transactions CSVs
- `merge_datasets(train, stores, oil, holidays, transactions)` — joins all sources
- `detect_outliers_iqr(df)` — IQR-based outlier flagging by store/family

### features.py: FastFeatureEngineer

Fluent API for feature engineering. Chain methods:

```python
fe = FastFeatureEngineer(df, transactions=tx_df, oil_price=oil_df, holidays=hol_df, store_meta=stores_df)
fe.add_temporal_features()
fe.add_lag_and_rolling(lags=[1,7,14], windows=[7,14,28])
fe.add_transaction_features()
fe.add_macroeconomic_features()
df = fe.transform()
```

Available methods: `add_temporal_features()`, `add_lag_and_rolling()`, `add_onpromotion_features()`, `add_macroeconomic_features()`, `add_transaction_features()`, `add_store_metadata()`, `add_cannibalization_features()`

### visualization.py

- `plot_ts_decomposition(df, store_nbr, family)` — seasonal decomposition
- `plot_correlation_heatmap(df)` — feature correlation
- `plot_sales_distribution(df)` — sales histogram

## Data

- `data/raw/` — original CSVs (gitignored)
- `data/processed/` — cleaned/featured datasets (gitignored)
- `outputs/plots/`, `outputs/models/`, `outputs/logs/` — generated artifacts (gitignored)

## Development Rules

1. **PATH_STRICT**: Use `config.py` constants for all file I/O
2. **MODULAR_ML**: Keep logic in `src/retail_iq/`, not notebooks
3. **NO_FLUFF**: Dense reasoning, no conversational filler
4. Sync `requirements.txt` and `pyproject.toml` before installing dependencies

## Tech Stack

pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels, xgboost, flask
