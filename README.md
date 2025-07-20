# Stochastic Forecasting & Signal System

A Python-based quantitative simulation engine for advanced stock price modeling using stochastic processes, technical indicators, and macroeconomic factor integration.

## Overview

This system implements an enhanced Geometric Brownian Motion (GBM) model with jump diffusion processes to forecast stock price movements over 2-year horizons. It integrates real-time momentum indicators, macroeconomic correlations, and comprehensive risk analysis to generate professional investment reports.

## Key Technical Features

### Advanced Stochastic Modeling
- **Enhanced GBM with Jump Diffusion**: 50,000 Monte Carlo simulations per stock
- **Dynamic Parameter Adjustment**: Drift and volatility modified by market momentum and macro factors
- **Jump Detection**: Automatic identification and modeling of 3-sigma market events

### Multi-Factor Integration
- **Technical Indicators**: RSI, MACD, Bollinger Bands, Moving Average convergence
- **Macroeconomic Factors**: VIX, 10-Year Treasury, S&P 500, Currency indices, Gold
- **Correlation Analysis**: Real-time sensitivity to market conditions

### Comprehensive Risk Analytics
- **Value at Risk (VaR)**: 5% worst-case scenarios
- **Conditional VaR (CVaR)**: Expected loss under tail risk
- **Maximum Drawdown**: Peak-to-trough loss analysis
- **Upside Potential**: 95th percentile gain estimates
- **Profit Probability**: Likelihood of positive returns

## Output Generation

### Excel Reports
- Cross-stock comparison dashboards
- Statistical price projections and return analysis
- Investment outcome simulations with dollar-based P&L
- Current momentum indicator values and model parameters

### Professional Visualizations
- Simulated price paths with confidence bands
- Price and return distribution histograms
- Risk metrics summary charts
- Momentum indicator analysis

## Technical Stack

- **Python**: NumPy, Pandas, SciPy for numerical computations
- **Data Sources**: Yahoo Finance API for real-time market data
- **Visualization**: Matplotlib, Seaborn for professional charts
- **Reporting**: Excel integration with xlsxwriter and openpyxl
- **Statistical Analysis**: Monte Carlo simulation, correlation analysis, jump detection

## Use Cases

- Portfolio risk assessment and optimization
- Investment research and due diligence
- Quantitative trading strategy development
- Academic research in financial modeling

## Project Status

Active development with continuous improvements to modeling accuracy, additional technical indicators, and machine learning integration planned.
