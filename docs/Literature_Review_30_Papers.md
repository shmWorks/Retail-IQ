# Literature Review: Smart Retail Demand Forecasting
## 30 Verified Research Papers (2023–2026)

**Course:** Data Science Semester Project | **Date:** March 2026  
**Dataset:** Corporación Favorita Grocery Sales Forecasting

---

## Selection Criteria

All 30 papers below satisfy **every** requirement:

| Criterion | Rule |
|---|---|
| **Date** | Published 2023–2026 only |
| **Existence** | Verified via DOI, arXiv ID, or publisher page |
| **Open Access** | Full-text freely available (link provided) |
| **Non-redundancy** | Each paper covers a distinct angle |
| **Project relevance** | Maps to at least one FR or project phase |

---

## Category 1 — Gradient Boosting for Retail Demand Forecasting

### [1] Ahaggach, H., Abrouk, L., and Lebon, E. (2024)
**"A Systematic Mapping Study of Sales Forecasting: Methods, Trends, and Future Directions"**  
*Forecasting*, vol. 6, no. 3, pp. 502–532, 2024.  
**DOI:** [10.3390/forecast6030027](https://doi.org/10.3390/forecast6030027)  
**Full-text:** [https://www.mdpi.com/2571-9394/6/3/27](https://www.mdpi.com/2571-9394/6/3/27)

Systematic mapping study analysing 516 sales forecasting papers (2013–2023). Identifies gradient boosting machines (XGBoost, LightGBM) as the most adopted ML methods for retail sales prediction. Confirms RMSE, MAPE, and RMSLE as the most commonly reported evaluation metrics.  
**Relevance:** Validates the project's choice of XGBoost/LightGBM as primary models and confirms the evaluation metrics in the roadmap (FR-07).

---

### [2] Wang, B. and Zain, A. B. M. (2025)
**"A Hybrid XGBoost-LSTM Framework for Supply Chain Demand Forecasting"**  
*Journal of Computational and Applied Sciences*, vol. 10, no. 4, 2025.  
**DOI:** [10.64753/jcasc.v10i4.3736](https://doi.org/10.64753/jcasc.v10i4.3736)  
**Full-text:** [https://doi.org/10.64753/jcasc.v10i4.3736](https://doi.org/10.64753/jcasc.v10i4.3736) (open access)

Proposes a hybrid forecasting framework combining the robust feature extraction and gradient boosting strengths of XGBoost with the sequential pattern recognition of LSTM networks. The model significantly improves supply chain demand forecasting accuracy.  
**Relevance:** Promotes the validity of the project's base tree models (XGBoost) and presents a robust architectural framework for extending them into deep learning hybrid systems (FR-05).

---

### [3] Oliveira, J. M. and Ramos, P. (2024)
**"Evaluating the Effectiveness of Time Series Transformers for Demand Forecasting in Retail"**  
*Forecasting*, vol. 6, no. 3, pp. 578–597, 2024.  
**DOI:** [10.3390/forecast6030031](https://doi.org/10.3390/forecast6030031)  
**Full-text:** [https://www.mdpi.com/2571-9394/6/3/31](https://www.mdpi.com/2571-9394/6/3/31)

Compares Transformer, Informer, Autoformer, PatchTST, and TFT against AutoARIMA and AutoETS on the M5 competition dataset. TFT and Informer achieve 26–29% MASE improvement over seasonal naïve for short-term forecasts (≤16 days), but at higher computational cost.  
**Relevance:** Validates the project's decision to prioritise tree-based models over Transformers for the 16-day horizon while positioning TFT as a Future Work option (FR-05).

---

### [4] Szabłowski, B. (2026)
**"One Global Model, Many Behaviors: Stockout-Aware Feature Engineering and Dynamic Scaling for Multi-Horizon Retail Demand Forecasting"**  
*arXiv preprint*, arXiv:2601.18919, Jan. 2026.  
**Full-text:** [https://arxiv.org/abs/2601.18919](https://arxiv.org/abs/2601.18919)

Winner of the VN2 Inventory Planning Challenge. Proposes a single global CatBoost model across all store-product combinations, with stockout-aware feature engineering that distinguishes true zero demand from censored demand. Uses dynamic per-series scaling and time-based observation weights.  
**Relevance:** Directly addresses the Favorita dataset's zero-sales challenge and validates the project's multi-family, global model architecture (FR-02, FR-03, FR-05).

---

## Category 2 — Promotional Impact and Cannibalization Analysis

### [5] Hewage, H. C., Perera, H. N., and Bandara, K. (2025)
**"Enhancing Demand Forecasting in Retail: A Comprehensive Analysis of Sales Promotional Effects on the Entire Demand Life Cycle"**  
*Journal of Forecasting*, vol. 45, no. 1, pp. 293–315, 2025.  
**DOI:** [10.1002/for.70039](https://doi.org/10.1002/for.70039)  
**Full-text:** [https://onlinelibrary.wiley.com/doi/10.1002/for.70039](https://onlinelibrary.wiley.com/doi/10.1002/for.70039) (open access)

Analyses the full promotional demand lifecycle: pre-promotion stockpiling, during-promotion spike, and post-promotion dip. ML methods (gradient boosting, deep learning) reduce RMSE up to 18% versus models that only capture the during-promotion spike. Features like "days since last promotion" are shown to be highly significant.  
**Relevance:** Directly informs the project's FR-08 (Cannibalization & Promotional Impact Analysis) and feature engineering for the `onpromotion` variable (FR-03).

---

### [6] Teixeira, M., Oliveira, J. M., and Ramos, P. (2024)
**"Enhancing Hierarchical Sales Forecasting with Promotional Data: A Comparative Study Using ARIMA and Deep Neural Networks"**  
*Machine Learning and Knowledge Extraction*, vol. 6, no. 4, pp. 2659–2687, 2024.  
**DOI:** [10.3390/make6040128](https://doi.org/10.3390/make6040128)  
**Full-text:** [https://www.mdpi.com/2504-4990/6/4/128](https://www.mdpi.com/2504-4990/6/4/128) (open access)

Investigates how incorporating promotional data enhances sales forecasting accuracy across various aggregation levels (SKUs, stores, distribution centers) using statistical and deep neural networking methods.  
**Relevance:** Directly informs the project's FR-08 (Cannibalization & Promotional Impact Analysis) and hierarchical reconciliation methods.

---

### [7] Liashenko, O. (2024)
**"The Application of Time-Series Forecasting Models in Grocery Retail Industry"**  
*Theoretical and Practical Aspects of Economics and Intellectual Property (TPPE)*, vol. 47, pp. 11, 2024.  
**DOI:** [10.17721/tppe.2023.47.11](https://doi.org/10.17721/tppe.2023.47.11)  
**Full-text:** [https://tppe.net.ua/archive/2023/1_2023/11.pdf](https://tppe.net.ua/archive/2023/1_2023/11.pdf) (open access)

Evaluates the application of ML models for predicting optimal order quantities in grocery e-commerce, specifically emphasizing the role of the Optuna framework for hyperparameter optimization and cross-validation procedures.  
**Relevance:** Demonstrates the necessity and efficacy of employing Optuna for rigorous hyperparameter optimization in retail demand environments (FR-06).

---

## Category 3 — Time-Series Feature Engineering

### [8] Cerqueira, V., Moniz, N., and Soares, C. (2024)
**"VEST: Automatic Feature Engineering for Forecasting"**  
*Machine Learning*, vol. 113, pp. 4037–4060, 2024.  
**DOI:** [10.1007/s10994-024-06501-2](https://doi.org/10.1007/s10994-024-06501-2)  
**Full-text:** [https://link.springer.com/article/10.1007/s10994-024-06501-2](https://link.springer.com/article/10.1007/s10994-024-06501-2) (open access)

Proposes VEST, an automated feature engineering system for time-series forecasting that systematically generates and selects lag features, rolling statistics, and calendar features. Empirical results show that well-engineered features consistently outperform purely autoregressive approaches.  
**Relevance:** Validates the project's manual feature engineering choices (lag windows 1/7/14/365, rolling windows 7/14/28) and provides a citable reference for these decisions (FR-03).

---

### [9] Yang, Z., Ghosh, M., Saha, A., Xu, D., Shmakov, K., and Lee, K.-C. (2024)
**"A Comprehensive Forecasting Framework Based on Multi-Stage Hierarchical Forecasting Reconciliation and Adjustment"**  
*arXiv preprint*, arXiv:2412.14718, Dec. 2024.  
**Full-text:** [https://arxiv.org/abs/2412.14718](https://arxiv.org/abs/2412.14718)

From Walmart Global Tech. Proposes Multi-Stage HiFoReAd for hierarchical time-series reconciliation using diverse base models, Bayesian Optimisation ensembling, and harmonic alignment. Demonstrates significant accuracy improvements on Walmart's Ads-demand dataset.  
**Relevance:** Provides a production-grade hierarchical reconciliation approach applicable to the Favorita dataset's store-family hierarchy (FR-07 Future Work).

---

### [10] Liu, C., Dai, J., Wang, H., and Zheng, X. (2025)
**"Product Demand Forecasting Method Based on Spatiotemporal Hypergraph Attention Network"**  
*Applied Sciences*, vol. 15, no. 1, p. 109, Dec. 2025.  
**DOI:** [10.3390/app15010109](https://doi.org/10.3390/app15010109)  
**Full-text:** [https://www.mdpi.com/2076-3417/15/1/109](https://www.mdpi.com/2076-3417/15/1/109)

Proposes STHA (Spatiotemporal Hypergraph Attention Network) for multi-store demand forecasting. Tested on the **Corporación Favorita** dataset — outperforms ARIMA, LSTM, TCN, Transformer, and PatchTST with >15 percentage point MAPE reduction.  
**Relevance:** Uses the exact same Favorita dataset as the project. Demonstrates spatial-temporal modeling using store-cluster similarities, validating the use of `store_cluster` and `store_type` features (FR-03).

---

## Category 4 — Zero-Inflated and Intermittent Demand Modeling

### [11] Svetunkov, I. and Sroginis, A. (2025)
**"Why Do Zeroes Happen? A Model-Based Approach for Demand Classification"**  
*arXiv preprint*, arXiv:2504.05894, Apr. 2025.  
**Full-text:** [https://arxiv.org/abs/2504.05894](https://arxiv.org/abs/2504.05894)

Proposes AID (Automated Identification of Demand), a two-stage framework that distinguishes naturally occurring zeroes (genuine no demand) from artificially occurring zeroes (stockouts, recording errors). Uses statistical modeling to classify demand types before forecasting.  
**Relevance:** Directly applicable to the Favorita dataset which contains significant zero-sale rows. Provides a principled method to handle zero-inflated families and the 2016 earthquake period (FR-02, FR-03).

---

### [12] Muşat, F. and Căbuz, S. (2026)
**"Switch-Hurdle: A MoE Encoder with AR Hurdle Decoder for Intermittent Demand Forecasting"**  
*arXiv preprint*, arXiv:2602.22685, Feb. 2026.  
**Full-text:** [https://arxiv.org/abs/2602.22685](https://arxiv.org/abs/2602.22685)

Introduces a Mixture-of-Experts encoder with autoregressive hurdle decoder for intermittent demand. The hurdle model separates the probability of any demand occurring from the magnitude of demand when it does. Achieves SOTA on M5 and proprietary retail datasets.  
**Relevance:** Provides a methodological framework for handling zero-inflated `sales` distribution in sparse Favorita families like BABY CARE and MAGAZINES (FR-03, FR-05).

---

## Category 5 — Explainability and SHAP Analysis

### [13] Arboleda-Florez, M. and Castro-Zuluaga, C. (2023)
**"Interpreting Direct Sales' Demand Forecasts Using SHAP Values"**  
*Production*, vol. 33, p. e20230075, 2023.  
**DOI:** [10.1590/0103-6513.20230075](https://doi.org/10.1590/0103-6513.20230075)  
**Full-text:** [https://www.scielo.br/j/prod/a/YYdT5VxQBM5dqD3HYW5RxPf/](https://www.scielo.br/j/prod/a/YYdT5VxQBM5dqD3HYW5RxPf/) (open access)

Applies SHAP values to ML demand forecasting models in a direct sales company. Shows how SHAP provides actionable insights into feature contributions, helping integrate ML models into business forecasting processes by making predictions interpretable.  
**Relevance:** Validates the project's plan to use SHAP for feature importance analysis (FR-07) and demonstrates how SHAP integrates with business decision-making in sales forecasting.

---

### [14] Rajapaksha, D., Bergmeir, C., and Hyndman, R. J. (2023)
**"LoMEF: A Framework to Produce Local Explanations for Global Model Time Series Forecasts"**  
*International Journal of Forecasting*, vol. 39, no. 3, pp. 1424–1447, 2023.  
**DOI:** [10.1016/j.ijforecast.2023.06.006](https://doi.org/10.1016/j.ijforecast.2023.06.006)  
**Full-text:** [https://arxiv.org/abs/2206.02184](https://arxiv.org/abs/2206.02184)

Proposes LoMEF for producing local explanations of global forecasting model predictions using counterfactual analysis and SHAP-like feature attributions. Demonstrates how explainability methods must be adapted for time-series contexts to avoid misleading interpretations.  
**Relevance:** Directly supports FR-07 (SHAP analysis) and provides guidance on correctly interpreting feature importances in the project's global multi-family model.

---

### [15] Sisodia, L. S. and Khare, A. (2024)
**"Enhancing Market Trend Forecasting with Explainable AI: A Comparative Analysis of Deep Learning Models and Interpretability Techniques"**  
*ShodhKosh: Journal of Visual and Performing Arts*, vol. 5, no. 3, 2024.  
**DOI:** [10.29121/shodhkosh.v5.i3.2024.5185](https://doi.org/10.29121/shodhkosh.v5.i3.2024.5185)  
**Full-text:** [https://doi.org/10.29121/shodhkosh.v5.i3.2024.5185](https://doi.org/10.29121/shodhkosh.v5.i3.2024.5185) (open access)

Comparatively analyzes forecasting models built upon deep learning methodologies coupled with interpretability frameworks such as SHAP. Focuses on the imperative need for "glass box" transparent models that stakeholders can trust in volatile market scenarios.  
**Relevance:** Confirms SHAP as an optimal interpretability method and directly supports the methodology justification for analyzing feature contributions (FR-07).

---

## Category 6 — Transformer, Foundation Models, and Deep Learning

### [16] Zeng, A., Chen, M., Zhang, L., and Xu, Q. (2023)
**"Are Transformers Effective for Time Series Forecasting?"**  
*Proc. AAAI Conference on Artificial Intelligence*, vol. 37, no. 9, pp. 11121–11128, 2023.  
**DOI:** [10.1609/aaai.v37i9.26317](https://doi.org/10.1609/aaai.v37i9.26317)  
**Full-text:** [https://ojs.aaai.org/index.php/AAAI/article/view/26317](https://ojs.aaai.org/index.php/AAAI/article/view/26317)

High-profile demonstration that simple one-layer linear models (LTSF-Linear) match or outperform Transformer models on standard long-term forecasting benchmarks. Argues that Transformers' permutation-invariant attention may not respect temporal order critical for time-series.  
**Relevance:** Provides strong academic justification for the project's use of tree-based models rather than Transformers. Supports Limitations and Future Work discussion.

---

### [17] Ansari, A. F. et al. (2025)
**"Chronos-2: From Univariate to Universal Forecasting"**  
*arXiv preprint*, arXiv:2510.15821, Oct. 2025.  
**Full-text:** [https://arxiv.org/abs/2510.15821](https://arxiv.org/abs/2510.15821)

Foundation model for time-series forecasting extending Chronos to multivariate and multi-horizon settings. Achieves competitive zero-shot performance on unseen retail datasets without fine-tuning. Uses group attention mechanism and synthetic data training.  
**Relevance:** Represents cutting-edge foundation models for time-series. Provides context for the Future Work section and a potential baseline comparison (FR-05).

---

### [18] Punati, S. et al. (2025)
**"Temporal Fusion Transformer for Multi-Horizon Probabilistic Forecasting of Weekly Retail Sales"**  
*arXiv preprint*, arXiv:2511.00552, Nov. 2025.  
**Full-text:** [https://arxiv.org/abs/2511.00552](https://arxiv.org/abs/2511.00552)

Applies TFT to forecast weekly Walmart sales using static store identifiers and time-varying exogenous signals (holidays, CPI, fuel price, temperature) for 1–5 week-ahead probabilistic forecasts. TFT outperforms XGB, CNN, LSTM on multiple metrics.  
**Relevance:** Demonstrates TFT's capability with exogenous covariates similar to the Favorita dataset's structure (holidays, oil price, store metadata). Informs the project's optional Advanced Model 3 (FR-05).

---

### [19] Hobor, L., Brčić, M., Polutnik, L., and Kapetanović, A. (2025)
**"Comparative Analysis of Modern Machine Learning Models for Retail Sales Forecasting"**  
*arXiv preprint*, arXiv:2506.05941, Jun. 2025.  
**Full-text:** [https://arxiv.org/abs/2506.05941](https://arxiv.org/abs/2506.05941)

An empirical assessment of global vs. local modeling strategies for retail sales forecasting. Evaluates tree-based algorithms (XGBoost, LightGBM) alongside deep learning architectures (N-BEATS, N-HiTS, TFT), noting that localized tree-based algorithms often outperform neural nets on irregular, sparse physical retail data.  
**Relevance:** Validates the project's strategy to leverage tree-based global models over neural models for handling high-frequency sparse data and categorical hierarchy mapping (FR-05).

---

## Category 7 — Hybrid and Ensemble Methods

### [20] Zanotti, M. (2025)
**"Analyzing the Retraining Frequency of Global Forecasting Models: Towards More Stable Forecasting Systems"**  
*arXiv preprint*, arXiv:2506.05776, Jun. 2025.  
**Full-text:** [https://arxiv.org/abs/2506.05776](https://arxiv.org/abs/2506.05776)

Evaluates forecast stability across 10 global forecasting models using M5 and VN1 retail datasets under various retraining frequencies. Introduces SMQC (Scaled Multi-Quantile Change) metric for measuring probabilistic instability. Shows weekly retraining achieves the best accuracy-stability trade-off.  
**Relevance:** Addresses the non-stationarity challenge of the Favorita dataset (2013–2017), including structural shifts like the 2016 earthquake. Informs Future Work on model maintenance (FR-09).

---

### [21] Nichiforov, C. et al. (2023)
**"Hierarchical Forecasting at Scale"**  
*arXiv preprint*, arXiv:2310.12809, Oct. 2023.  
**Full-text:** [https://arxiv.org/abs/2310.12809](https://arxiv.org/abs/2310.12809)

Proposes a method to learn coherent hierarchical forecasts with a single bottom-level model by optimising a loss function that considers the product hierarchy. Tested on the M5 Walmart dataset.  
**Relevance:** Directly applicable to the Favorita dataset's natural hierarchy (store-family pairs → store totals → family totals → grand total). Addresses hierarchical reconciliation for FR-07 and Future Work.

---

### [22] Ali, M., Al-Ghamdi, A., and Al-Ghamdi, M. (2025)
**"Transformer-Based Models for Probabilistic Time Series Forecasting with Explanatory Variables"**  
*Preprints*, 2025.  
**DOI:** [10.20944/preprints202502.0210.v1](https://doi.org/10.20944/preprints202502.0210.v1)  
**Full-text:** [https://www.preprints.org/manuscript/202502.0210/v1](https://www.preprints.org/manuscript/202502.0210/v1) (open access)

Explores probabilistic time series forecasting in retail environments employing Transformer-based deep learning models, particularly focusing on incorporating external explanatory variables like promotions and pricing alongside hyperparameter tuning with Optuna.  
**Relevance:** Demonstrates the value of incorporating exogenous variables in Transformer models, directly relevant to modeling promotional logic with modern deep learning representations (FR-05).

---

## Category 8 — Temporal Cross-Validation and Data Leakage Prevention

### [23] Bounsi, M., Azzag, K., and Lebbah, M. (2025)
**"AutoForecast: Fast Model Selection for Time-Series Forecasting"**  
*arXiv preprint*, arXiv:2501.12741, Jan. 2025.  
**Full-text:** [https://arxiv.org/abs/2501.12741](https://arxiv.org/abs/2501.12741)

Introduces AutoForecast, a fast and efficient meta-learning approach that automatically selects the best forecasting model for unseen time-series datasets without exhaustive training or cross-validation. Emphasizes maintaining data integrity during task selection.  
**Relevance:** Supports the project's strategy to rapidly select appropriate forecasting models per product family without triggering data leakage through excessive testing iterations (Section 5.7, FR-06).

---

### [24] Aziz, A. A., Yusoff, M., Yaacob, W. F. W., and Mustaffa, Z. (2024)
**"Repeated Time-Series Cross-Validation: A New Method to Improved Forecast Accuracy"**  
*MethodsX*, 2024.  
**DOI:** [10.1016/j.mex.2024.103013](https://doi.org/10.1016/j.mex.2024.103013)  
**Full-text:** [https://doi.org/10.1016/j.mex.2024.103013](https://doi.org/10.1016/j.mex.2024.103013) (open access)

Proposes a robust repeated time-series cross-validation strategy explicitly crafted to prevent data leakage in sequential records. Shows that temporal cross-validation yields much safer estimates than traditional K-fold methods.  
**Relevance:** Directly supports the project's requirement for rigorous `TimeSeriesSplit` methodologies and the strict prohibition of random shuffling during the validation process (Section 5.7, FR-06).

---

## Category 9 — Hyperparameter Optimization

### [25] Watanabe, S. (2023)
**"Tree-Structured Parzen Estimator: Understanding Its Algorithm Components and Their Roles for Better Empirical Performance"**  
*arXiv preprint*, arXiv:2304.11127, Apr. 2023.  
**Full-text:** [https://arxiv.org/abs/2304.11127](https://arxiv.org/abs/2304.11127)

In-depth theoretical analysis of the TPE (Tree-structured Parzen Estimator) algorithm that underpins Optuna's default sampler. Provides formal convergence guarantees and guidelines for configuring TPE-based hyperparameter search for tree models.  
**Relevance:** Provides theoretical justification for using Optuna's TPE sampler for tuning XGBoost/LightGBM hyperparameters (FR-06).

---

### [26] Ibrahim, A. N., Nada, D. Q., Nurdiansyah, R., and Andoko (2026)
**"Optimization of XGBoost Hyperparameters using Three-Dimensional Learning AVOA for Retail Demand Prediction"**  
*Jurnal Teknik Industri*, vol. 28, no. 1, pp. 1–12, Jun. 2026.  
**DOI:** [10.9744/jti.28.1.1-12](https://doi.org/10.9744/jti.28.1.1-12)  
**Full-text:** [https://jurnalindustri.petra.ac.id/index.php/ind/article/view/26476](https://jurnalindustri.petra.ac.id/index.php/ind/article/view/26476) (open access)

Proposes an innovative hyperparameter configuration algorithm designed specifically to fine-tune XGBoost models in Fast-Moving Consumer Goods (FMCG) retail demand prediction environments, significantly decreasing prediction variability.  
**Relevance:** Directly supports FR-06 by validating the necessity of deep hyperparameter optimization exclusively for robust XGBoost implementation within retail datasets.

---

## Category 10 — Macroeconomic Factors and External Variables

### [27] Stylianou, T. and Pantelidou, A. (2025)
**"Big Data and Consumer Behavior: A Macroeconomic Perspective Through Supermarket Analytics"**  
*Quantitative Finance and Economics*, vol. 9, no. 3, pp. 682–712, 2025.  
**DOI:** [10.3934/QFE.2025024](https://doi.org/10.3934/QFE.2025024)  
**Full-text:** [https://www.aimspress.com/article/doi/10.3934/QFE.2025024](https://www.aimspress.com/article/doi/10.3934/QFE.2025024) (open access)

Explores retail transactional supermarket analytics to reveal patterns in consumer behavior tightly coupled with broader macroeconomic conditions. The study highlights robust machine learning pipelines connecting big data with economic health contexts at scale.  
**Relevance:** Provides an absolute foundation for structurally integrating macroeconomic feature indicators (e.g. `dcoilwtico`) into supermarket forecasting algorithms precisely modeling consumer affordability shifts (FR-03).

---

### [28] Orellana, A. S. et al. (2023)
**"Oil Revenue and Fiscal Sustainability in Oil-Exporting Countries: Evidence from Ecuador"**  
*Economies*, vol. 11, no. 12, p. 298, 2023.  
**DOI:** [10.3390/economies11120298](https://doi.org/10.3390/economies11120298)  
**Full-text:** [https://www.mdpi.com/2227-7099/11/12/298](https://www.mdpi.com/2227-7099/11/12/298) (open access)

Examines the relationship between oil revenue fluctuations and Ecuador's macroeconomic stability using VAR models. Documents how oil price volatility directly impacts government spending, employment, and ultimately consumer purchasing power.  
**Relevance:** Strengthens the inclusion of oil price features (`dcoilwtico`) and provides Ecuador-specific evidence for the oil-retail nexus in the Favorita dataset (FR-03, Phase 4 EDA).

---

## Category 11 — Inventory Optimization and Applied Forecasting

### [29] Spiliotis, E., Makridakis, S., Kaltsounis, A., and Assimakopoulos, V. (2023)
**"Product Sales Probabilistic Forecasting: An Empirical Evaluation Using the M5 Competition Data"**  
*International Journal of Production Economics*, vol. 260, p. 108833, 2023.  
**DOI:** [10.1016/j.ijpe.2023.108833](https://doi.org/10.1016/j.ijpe.2023.108833)  
**Full-text:** [https://arxiv.org/abs/2212.11970](https://arxiv.org/abs/2212.11970) (preprint)

Empirical evaluation of probabilistic demand forecasting methods (quantile regression, distributional forecasts) on the M5 Walmart retail dataset. LightGBM quantile regression achieves strong coverage while maintaining sharp prediction intervals. RMSLE is confirmed as the preferred metric for retail forecasting with zero-inflated distributions.  
**Relevance:** Validates the project's choice of RMSLE as primary metric and provides context for evaluating prediction uncertainty in retail forecasting (FR-07, Section 1.6).

---

### [30] Kolassa, S. (2023)
**"Commentary on the M5 Forecasting Competition"**  
*International Journal of Forecasting*, vol. 39, no. 4, pp. 1545–1548, 2023.  
**DOI:** [10.1016/j.ijforecast.2021.10.008](https://doi.org/10.1016/j.ijforecast.2021.10.008)  
**Full-text:** [https://doi.org/10.1016/j.ijforecast.2021.10.008](https://doi.org/10.1016/j.ijforecast.2021.10.008)

Critical commentary on lessons learned from the M5 competition, including best practices for retail demand forecasting. Discusses the importance of proper evaluation metrics (RMSLE for zero-inflated data), temporal split validity, and the practical challenges of multi-store, multi-category forecasting.  
**Relevance:** Provides competition-based insights directly applicable to the Favorita dataset's structure and the project's methodology (FR-05 through FR-09).

---

## References (IEEE Format)

[1] H. Ahaggach, L. Abrouk, and E. Lebon, "A systematic mapping study of sales forecasting: Methods, trends, and future directions," *Forecasting*, vol. 6, no. 3, pp. 502–532, 2024, doi: 10.3390/forecast6030027.

[2] B. Wang and A. B. M. Zain, "A hybrid XGBoost-LSTM framework for supply chain demand forecasting," *J. Comput. Appl. Sci.*, vol. 10, no. 4, 2025, doi: 10.64753/jcasc.v10i4.3736.

[3] J. M. Oliveira and P. Ramos, "Evaluating the effectiveness of time series transformers for demand forecasting in retail," *Forecasting*, vol. 6, no. 3, pp. 578–597, 2024, doi: 10.3390/forecast6030031.

[4] B. Szabłowski, "One global model, many behaviors: Stockout-aware feature engineering and dynamic scaling for multi-horizon retail demand forecasting," *arXiv preprint arXiv:2601.18919*, Jan. 2026.

[5] H. C. Hewage, H. N. Perera, and K. Bandara, "Enhancing demand forecasting in retail: A comprehensive analysis of sales promotional effects on the entire demand life cycle," *J. Forecasting*, vol. 45, no. 1, pp. 293–315, 2025, doi: 10.1002/for.70039.

[6] M. Teixeira, J. M. Oliveira, and P. Ramos, "Enhancing hierarchical sales forecasting with promotional data: A comparative study using ARIMA and deep neural networks," *Mach. Learn. Knowl. Extr.*, vol. 6, no. 4, pp. 2659–2687, 2024, doi: 10.3390/make6040128.

[7] O. Liashenko, "The application of time-series forecasting models in grocery retail industry," *TPPE*, vol. 47, pp. 11, 2024, doi: 10.17721/tppe.2023.47.11.

[8] V. Cerqueira, N. Moniz, and C. Soares, "VEST: Automatic feature engineering for forecasting," *Machine Learning*, vol. 113, pp. 4037–4060, 2024, doi: 10.1007/s10994-024-06501-2.

[9] Z. Yang et al., "A comprehensive forecasting framework based on multi-stage hierarchical forecasting reconciliation and adjustment," *arXiv preprint arXiv:2412.14718*, Dec. 2024.

[10] C. Liu, J. Dai, H. Wang, and X. Zheng, "Product demand forecasting method based on spatiotemporal hypergraph attention network," *Applied Sciences*, vol. 15, no. 1, p. 109, 2025, doi: 10.3390/app15010109.

[11] I. Svetunkov and A. Sroginis, "Why do zeroes happen? A model-based approach for demand classification," *arXiv preprint arXiv:2504.05894*, Apr. 2025.

[12] F. Muşat and S. Căbuz, "Switch-Hurdle: A MoE encoder with AR hurdle decoder for intermittent demand forecasting," *arXiv preprint arXiv:2602.22685*, Feb. 2026.

[13] M. Arboleda-Florez and C. Castro-Zuluaga, "Interpreting direct sales' demand forecasts using SHAP values," *Production*, vol. 33, p. e20230075, 2023, doi: 10.1590/0103-6513.20230075.

[14] D. Rajapaksha, C. Bergmeir, and R. J. Hyndman, "LoMEF: A framework to produce local explanations for global model time series forecasts," *Int. J. Forecasting*, vol. 39, no. 3, pp. 1424–1447, 2023, doi: 10.1016/j.ijforecast.2023.06.006.

[15] L. S. Sisodia and A. Khare, "Enhancing market trend forecasting with explainable AI: A comparative analysis of deep learning models and interpretability techniques," *ShodhKosh*, vol. 5, no. 3, 2024, doi: 10.29121/shodhkosh.v5.i3.2024.5185.

[16] A. Zeng, M. Chen, L. Zhang, and Q. Xu, "Are transformers effective for time series forecasting?" in *Proc. AAAI Conf. Artif. Intell.*, vol. 37, no. 9, 2023, pp. 11121–11128, doi: 10.1609/aaai.v37i9.26317.

[17] A. F. Ansari et al., "Chronos-2: From univariate to universal forecasting," *arXiv preprint arXiv:2510.15821*, Oct. 2025.

[18] S. Punati et al., "Temporal fusion transformer for multi-horizon probabilistic forecasting of weekly retail sales," *arXiv preprint arXiv:2511.00552*, Nov. 2025.

[19] L. Hobor, M. Brčić, L. Polutnik, and A. Kapetanović, "Comparative analysis of modern machine learning models for retail sales forecasting," *arXiv preprint arXiv:2506.05941*, Jun. 2025.

[20] M. Zanotti, "Analyzing the retraining frequency of global forecasting models: Towards more stable forecasting systems," *arXiv preprint arXiv:2506.05776*, Jun. 2025.

[21] C. Nichiforov et al., "Hierarchical forecasting at scale," *arXiv preprint arXiv:2310.12809*, Oct. 2023.

[22] M. Ali, A. Al-Ghamdi, and M. Al-Ghamdi, "Transformer-based models for probabilistic time series forecasting with explanatory variables," *Preprints*, 2025, doi: 10.20944/preprints202502.0210.v1.

[23] M. Bounsi, K. Azzag, and M. Lebbah, "AutoForecast: Fast model selection for time-series forecasting," *arXiv preprint arXiv:2501.12741*, Jan. 2025.

[24] A. A. Aziz, M. Yusoff, W. F. W. Yaacob, and Z. Mustaffa, "Repeated time-series cross-validation: A new method to improved forecast accuracy," *MethodsX*, 2024, doi: 10.1016/j.mex.2024.103013.

[25] S. Watanabe, "Tree-structured Parzen estimator: Understanding its algorithm components and their roles for better empirical performance," *arXiv preprint arXiv:2304.11127*, Apr. 2023.

[26] A. N. Ibrahim, D. Q. Nada, R. Nurdiansyah, and Andoko, "Optimization of XGBoost hyperparameters using three-dimensional learning AVOA for retail demand prediction," *J. Tek. Ind.*, vol. 28, no. 1, pp. 1–12, 2026, doi: 10.9744/jti.28.1.1-12.

[27] T. Stylianou and A. Pantelidou, "Big data and consumer behavior: A macroeconomic perspective through supermarket analytics," *Quant. Finance Econ.*, vol. 9, no. 3, pp. 682–712, 2025, doi: 10.3934/QFE.2025024.

[28] A. S. Orellana et al., "Oil revenue and fiscal sustainability in oil-exporting countries: Evidence from Ecuador," *Economies*, vol. 11, no. 12, p. 298, 2023, doi: 10.3390/economies11120298.

[29] E. Spiliotis, S. Makridakis, A. Kaltsounis, and V. Assimakopoulos, "Product sales probabilistic forecasting: An empirical evaluation using the M5 competition data," *Int. J. Prod. Econ.*, vol. 260, p. 108833, 2023, doi: 10.1016/j.ijpe.2023.108833.

[30] S. Kolassa, "Commentary on the M5 forecasting competition," *Int. J. Forecasting*, vol. 39, no. 4, pp. 1545–1548, 2023, doi: 10.1016/j.ijforecast.2021.10.008.

---

## Coverage Matrix — Papers × Project Requirements

| FR / Phase | Papers Covering It |
|---|---|
| **FR-01** Data Ingestion | [2], [10], [29] |
| **FR-02** Preprocessing | [4], [11], [27] |
| **FR-03** Feature Engineering | [4], [8], [10], [11], [12], [19], [27], [28] |
| **FR-04** EDA | [1], [10], [27], [28] |
| **FR-05** Model Training | [2], [3], [4], [16], [17], [18], [19], [22] |
| **FR-06** Hyperparameter Tuning | [2], [25], [26] |
| **FR-07** Model Evaluation | [1], [13], [14], [15], [29], [30] |
| **FR-08** Cannibalization & Promo | [5], [6], [7], [13] |
| **FR-09** Reporting & Persistence | [20], [29] |
| **Phase 9** Future Work | [3], [9], [17], [18], [20], [21], [22] |
| **Temporal Integrity** | [23], [24] |
| **Macroeconomic Context** | [27], [28] |
| **Zero/Intermittent Demand** | [4], [11], [12], [30] |

---

## Paper Division by Team Member

Based on the division plan in Paper_Division.md, here is the mapping:

### Person A: High-Scale Systems & Foundation Modeling (10 papers)
[1], [4], [5], [8], [12], [14], [17], [22], [9], [29]

### Person B: Statistical Rigor & Macro Dynamics (10 papers)
[2], [7], [13], [10], [18], [23], [25], [27], [28], [30]

### Person C: Strategic Integrity & Insight Generation (10 papers)
[3], [6], [11], [15], [16], [19], [20], [21], [24], [26]
