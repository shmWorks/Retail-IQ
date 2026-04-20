# Retail-IQ: Professional Retail Forecasting System

## 📌 Overview
Retail-IQ is a machine learning-based sales forecasting system built with software engineering best practices. It uses a modular architecture to handle large-scale time-series data, feature engineering, and automated reporting.

## 📂 Project Structure
```
Retail-IQ/
├── data/
│   ├── raw/                # Unmodified input CSVs
│   └── processed/          # Cleaned and featured datasets
├── docs/                   # Project documentation and reports
├── notebooks/              # Jupyter notebooks for experimentation
├── outputs/
│   ├── figures/            # Generated plots and visualizations
│   ├── models/             # Serialized model files (.pkl, .json)
│   └── logs/               # Processing and error logs
├── src/
│   └── retail_iq/          # Core Python package
│       ├── config.py       # Centralized path and config management
│       ├── preprocessing.py # Data loading and cleaning
│       ├── features.py      # Feature engineering logic
│       └── visualization.py # Plotting utilities
├── tests/                  # Unit and integration tests
├── pyproject.toml          # Project metadata and dependencies
└── requirements.txt        # Legacy dependency list
```

## 🚀 Getting Started

### 1. Setup Environment
```bash
# Using uv (recommended)
uv venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows
uv pip install -e .
```

### 2. Run Analysis
Open `notebooks/eda.ipynb` and run all cells to generate the initial EDA reports.

## 🛠 Tech Stack
- **ML**: Scikit-learn, XGBoost, Statsmodels
- **Data**: Pandas, NumPy
- **Visuals**: Matplotlib, Seaborn
- **API**: Flask
- **DevOps**: Pathlib (Robust Paths), Setuptools (Package management)
