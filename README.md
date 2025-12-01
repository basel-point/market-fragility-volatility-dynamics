# Fragility in Low-Volatility Regimes (1990–2025)
### Supporting Code & Figures for “How Stability Creates Market Instability”

This repository contains the public-facing analysis, figures, and cleaned notebooks accompanying the research article:

🔗 **How Stability Creates Market Instability**  
https://thebaselpoint.substack.com/

The project explores how prolonged low-volatility regimes quietly reshape market fragility. Using data from 1990–2025, the analysis focuses on three empirical mechanisms:

1. **Regime-dependent forecastability** — why standard volatility models (e.g., GARCH) fail abruptly once the market exits a calm regime.  
2. **Tail-dependent behavior** — how downside extremes widen and become more nonlinear even while average volatility remains low.  
3. **Crowding and leverage** — why surface indicators such as the VIX, credit spreads, and margin debt often fail to detect fragility until the unwind.

The core metric used throughout the analysis is the forecast-error gap between realized and implied volatility:

FE_t = | RV_t – VIX_t |


This repository provides a curated, redacted version of the analysis used to produce the figures in the article.

---

## Repository Structure
fragility-in-low-volatility-regimes/
│
├── figures/
│ ├── vix_vs_rv_fe.png
│ ├── garch_vs_ml_mae.png
│ ├── tail_vs_nontail_boxplot.png
│ ├── margin_scatterplot.png
│ ├── table_forecast_errors.png
│ └── table_tail_errors.png
│
├── notebooks/
│ ├── Hypothesis_3A_Forecastability_Redacted.ipynb
│ ├── Hypothesis_3B_TailBehavior_Redacted.ipynb
│ └── Hypothesis_3C_Crowding_Redacted.ipynb
│
└── README.md

---

## 🧪 Notebook Notes (Redacted)

The notebooks in this repo are demonstration versions of the analysis.  
To protect proprietary modeling logic and data sources, the following have been removed:

- API keys and credential access  
- raw datasets and CSV files  
- internal feature engineering steps  
- custom modeling functions  
- exploratory and abandoned drafts  

Where applicable, cells have been replaced with:

```python
# Redacted: proprietary modeling code removed for public release.

he visible cells include:

figure generation

FE_t construction logic

basic data handling

descriptive analysis used in the article

This format follows common practice for public research notes.

📊 Figures

All major figures and tables used in the article are provided in PNG format, including:

VIX vs Realized Volatility with Forecast-Error Gap

GARCH(1,1) vs Machine Learning forecast comparisons

Tail vs non-tail error distributions

Margin debt vs FE_t scatterplot

Summary tables of MAE and RMSE across regimes

Access these files in the figures/ directory.

🔍 Data Sources

The analysis draws from publicly accessible sources such as:

FRED (Federal Reserve Bank of St. Louis)

Yahoo Finance (yfinance)

Author-constructed datasets for forecast errors and model outputs

Raw data is not included in this repository due to licensing and reproducibility constraints.

📝 Citation

If referencing this work, please cite:

Kim, S.Y. (2025). How Stability Creates Market Instability. The Basel Point.

📬 Contact

For inquiries related to this research:

S.Y. Kim
The Basel Point
(Add your professional website or contact email if desired.)

⚠️ License

This repository is distributed for educational and informational purposes only.
Not investment advice. No warranties or guarantees of accuracy.
