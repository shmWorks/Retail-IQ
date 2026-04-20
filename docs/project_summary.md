# 🚀 Retail-IQ: Hyper-Agent Manifest (SPOT v2.0)

> [!IMPORTANT]
> **AGENT_PROTOCOL**: Read this file first. Use the `[API]` manifest to plan tasks without reading source files. Update `[STATE]` after every major turn.

## [META]
*   **Goal**: Time-series forecasting for Favorita sales using XGBoost.
*   **Arch**: Modular Python Package (`retail_iq`).
*   **Stack**: Python 3.10, XGBoost, Scikit-learn, Flask.

## [STATE]
*   **PHASE**: 3 (Insight/EDA) -> 4 (Learning/Training)
*   **STATUS**: Dataset refactored, modularized, and EDA plots generated.
*   **ACTIVE_TASK**: Transitioning to model training.
*   **BLOCKERS**: None.

## [API_MANIFEST]
| File | Members (Signatures) | Description |
| :--- | :--- | :--- |
| `config.py` | `PROJECT_ROOT`, `DATA_DIR`, `LOG_DIR`, `PLOT_DIR` | Path constants (Pathlib). |
| `preprocessing.py` | `load_raw_data()`, `preprocess_dates(dfs)`, `clean_oil_prices(oil_df)`, `merge_datasets(tr, st, oil, hol, tx)`, `detect_outliers_iqr(df)` | Raw ingestion to merged df. |
| `features.py` | `FastFeatureEngineer(df, tx, oil, hol, st)`<br>`.add_temporal_features()`, `.add_lag_and_rolling()`, `.add_onpromotion_features()`, `.add_macroeconomic_features()`, `.add_transaction_features()`, `.add_store_metadata()`, `.add_cannibalization_features()` | Class for feature pipeline. |
| `visualization.py` | `plot_ts_decomposition(df, s, f)`, `plot_correlation_heatmap(df)`, `plot_sales_distribution(df)` | Automated plotting. |

## [INDEX]
*   `data/raw/`: Original Kaggle CSVs (GitIgnored).
*   `notebooks/eda.ipynb`: Interactive analysis driver.
*   `outputs/`: Figures, logs, models (GitIgnored).
*   `tests/`: Unit/integration testing suite.
*   `REFLECTIONS.md`: Design logic and lessons.
*   `pyproject.toml`: Package/build configuration.

## [RULES]
1.  **NO_FLUFF**: Keep reasoning dense. Avoid conversational filler.
2.  **API_FIRST**: Use signatures from `[API_MANIFEST]` before opening files.
3.  **PATH_STRICT**: Always use `config.py` constants for file I/O.
4.  **STATE_UPDATE**: Append task completion to `[STATE]` if it changes project phase.
