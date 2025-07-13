# Stochastic Forecasting & Signal System

**Stochastic Forecasting & Signal System** is a Python-based quantitative simulation engine designed to model future stock price movements using advanced stochastic techniques, technical momentum indicators, macroeconomic sensitivity, and jump diffusion modeling. 

The system generates a comprehensive Excel report and professional-grade visualizations for each stock analyzed. This tool is suitable for research, portfolio analysis, or applied quantitative finance environments.

---

## Project Overview

This system uses a refined version of the Geometric Brownian Motion (GBM) model, enhanced by real-world momentum indicators and macroeconomic correlations. It captures both smooth trends and sudden shocks using jump diffusion processes and integrates risk analysis metrics such as Value-at-Risk (VaR) and Conditional VaR (CVaR).

---

## Key Features

### GBM with Multiple Factors
- **Dynamic Parameter Adjustment**: Drift and volatility are modified based on current market momentum and macro correlations.
- **Monte Carlo Engine**: 50,000 stochastic paths over a 2-year projection horizon for each stock.

### Advanced Momentum Integration
- **RSI (Relative Strength Index)**: Detects overbought/oversold conditions.
- **MACD (Moving Average Convergence Divergence)**: Captures trend momentum and signal crossovers.
- **Bollinger Bands**: Measures price deviation from volatility envelope.
- **Moving Average Momentum**: 50-day vs 200-day MA convergence signals.
- **Price vs MA**: Compares current price against short- and long-term moving averages.

### Macroeconomic Factor Integration
- **VIX (Volatility Index)**: Gauges market fear and uncertainty.
- **10-Year Treasury (TNX)**: Measures sensitivity to interest rate shifts.
- **S&P 500 (SPY)**: Captures systematic market beta.
- **Dollar Index (EUR/USD proxy)**: Assesses currency impact on stock behavior.
- **Gold (GLD)**: Serves as a macro risk-off proxy.

### Jump Diffusion Modeling
- **Automatic Jump Detection**: Identifies 3-sigma return events.
- **Jump Parameter Estimation**: Models jump frequency, average size, and volatility.

### Comprehensive Risk Analysis
- **Value at Risk (5%)**: Worst-case downside scenarios.
- **Conditional VaR (CVaR)**: Expected loss under tail risk.
- **Maximum Drawdown**: Largest simulated loss from peak to trough.
- **Upside Potential**: 95th percentile gain estimate.
- **Profit Probability**: Likelihood of ending in profit after 2 years.

---

## Output Summary

### Excel Report
Each run generates a full Excel workbook with:
- **Summary Dashboard**: Cross-stock comparison table.
- **Price Projections**: Statistical breakdown of price simulations.
- **Return Analysis**: Total and annualized returns with percentiles.
- **Investment Outcomes**: Dollar-based P&L simulations.
- **Momentum Indicators**: Current technical signal values.
- **Model Parameters**: Drift, volatility, jump stats, and adjustments.

### Visualizations
For each stock, six high-resolution charts are generated:
1. **Simulated Price Paths** with confidence bands
2. **Final Price Distribution** histogram
3. **Total Return Distribution**
4. **Profit/Loss Scenarios**
5. **Current Momentum Indicator Bar Chart**
6. **Risk Metrics Summary**

---

## How It Works

1. **Data Collection**  
   Pulls 5 years of historical stock and macroeconomic data via Yahoo Finance.

2. **Momentum Analysis**  
   Computes RSI, MACD, Bollinger Bands, MA convergence, and price signals.

3. **Macro Correlation**  
   Calculates daily return correlations to macroeconomic benchmarks.

4. **Jump Detection**  
   Uses 3-standard deviation filter to detect and model rare market events.

5. **Parameter Adjustment**  
   Updates GBM parameters (μ, σ) using both momentum and macro factors.

6. **Simulation**  
   Runs 50,000 Monte Carlo paths with optional jump diffusion overlay.

7. **Risk Assessment & Visualization**  
   Calculates risk metrics and creates charts for inclusion in Excel report.

8. **Report Generation**  
   All results, visuals, and insights are exported into a professional Excel file.

---

## Example Use Case

Suppose you want to simulate a 2-year outlook for a portfolio of 8 stocks including `GOOG`, `VFV`, and `BNS`. After running the script:

- You’ll receive a full Excel workbook with charts and tables
- You can visualize risk and return across your portfolio
- You’ll interpret current momentum signals alongside statistical forecasts
- You can make allocation decisions based on simulated P&L scenarios and drawdown risk

---

## ✅ Status

> **In Active Development** – continuously improved with additional indicators, scenario interpretation, and machine learning modules coming soon.

---
