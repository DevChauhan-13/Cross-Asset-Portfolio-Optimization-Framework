# Portfolio Optimization & Backtesting Framework

This project implements a quantitative portfolio optimization and backtesting framework to analyze how asset universe size impacts diversification, risk, and performance. We compare a **10-asset traditional portfolio** with a **12-asset extended portfolio** that includes higher-volatility assets.

---

## 📌 Problem Statement

The objective is to evaluate portfolio construction techniques under different asset universes and study their behavior in terms of risk-adjusted returns, drawdowns, and robustness during volatile periods.

---

## 📊 Data Description

- Input data consists of historical price-related information for multiple assets.
- Each dataset includes:
  - Open, High, Low prices
  - Percentage returns
  - Volume
  - Timestamps
- Two portfolio universes are constructed:
  - **10-Asset Portfolio** (traditional assets only)
  - **12-Asset Portfolio** (traditional + additional assets)

---

## 🛠 Data Preprocessing

- Timestamp alignment across assets
- Handling missing values
- Computation of daily log returns
- Alignment of return series for multi-asset analysis
- Visualization of:
  - Return distributions
  - Rolling volatility
  - Asset correlations

---

## 🧠 Model Overview

The following portfolio construction strategies are implemented:

- **Minimum Variance Portfolio**
- **Markowitz Mean-Variance Optimization (Maximum Sharpe)**
- **Risk Parity Portfolio**

For each portfolio universe, the annualized mean return vector (μ) and covariance matrix (Σ) are estimated and used as model inputs.

---

## ⚙️ Backtesting Framework

- Fixed-weight portfolios with periodic rebalancing
- Identical backtest periods for fair comparison
- Portfolio value computed using weighted returns
- Transaction costs assumed to be zero (unless specified)

---

## 📈 Evaluation Metrics

Performance is evaluated using:

- Annualized Sharpe Ratio
- Sortino Ratio
- Volatility
- Maximum Drawdown
- Correlation Heatmap
- Stress-test performance during high-volatility regimes
- Rolling Sharpe Ratio

---

## 📉 Results & Visualization

The framework generates:

- Equity curves
- Drawdown curves
- KPI summary tables
- Rolling performance metrics

These results enable direct comparison between different strategies and asset universes.

---

## ✅ Key Findings

- Larger asset universes improve diversification but may increase volatility.
- Risk Parity offers better drawdown control in stressed markets.
- Mean-Variance portfolios are sensitive to covariance estimation.
- Asset selection plays a critical role in portfolio robustness.

---

## 🚀 Possible Improvements

- Incorporating transaction costs and slippage
- Dynamic or regime-based rebalancing
- Robust covariance estimation techniques
- Extension to factor-based or ML-driven strategies

---

## 📂 Project Structure


---

## 🧾 Requirements

- Python 3.x
- NumPy
- Pandas
- Matplotlib / Seaborn
- SciPy

---

## 📜 License

This project is for academic and educational purposes.
