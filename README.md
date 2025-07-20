# Stochastic Forecasting & Signal System

A Python-based quantitative simulation engine for advanced stock price modeling using enhanced Geometric Brownian Motion (GBM) with jump diffusion processes, technical momentum indicators, and macroeconomic factor integration.

## Overview

This system implements an enhanced GBM model with jump diffusion to forecast stock price movements over 2-year horizons. It dynamically adjusts drift and volatility parameters based on real-time momentum indicators and macroeconomic correlations, generating comprehensive investment reports with professional visualizations.

## Key Technical Features

### Enhanced GBM with Jump Diffusion
- **50,000 Monte Carlo Simulations**: Per stock over 2-year projection period
- **Dynamic Parameter Adjustment**: Drift (μ) and volatility (σ) modified by momentum and macro factors
- **Jump Detection**: Automatic identification of 3-standard deviation market events
- **Jump Parameter Estimation**: Models jump frequency (λ), average size (μ_jump), and volatility (σ_jump)

### Technical Momentum Integration
- **RSI (Relative Strength Index)**: Overbought/oversold detection with momentum adjustment
- **MACD (Moving Average Convergence Divergence)**: Trend momentum and signal crossovers
- **Bollinger Bands Position**: Price deviation from volatility envelope
- **Moving Average Momentum**: 50-day vs 200-day MA convergence signals
- **Price vs Moving Averages**: Current price comparison against MA50 and MA200

### Macroeconomic Factor Integration
- **VIX (Volatility Index)**: Market fear and uncertainty correlation
- **10-Year Treasury (TNX)**: Interest rate sensitivity analysis
- **S&P 500 (SPY)**: Systematic market beta correlation
- **Gold (GLD)**: Macro risk-off proxy correlation
- **Real-time Correlation Analysis**: Daily return correlations to macro benchmarks

### Comprehensive Risk Analytics
- **Value at Risk (VaR)**: 5% worst-case downside scenarios
- **Conditional VaR (CVaR)**: Expected loss under tail risk conditions
- **Maximum Drawdown**: Largest simulated loss from peak to trough
- **Upside Potential**: 95th percentile gain estimates
- **Profit Probability**: Likelihood of positive returns after 2 years
- **Investment Outcomes**: Dollar-based P&L simulations with share calculations

## Output Generation

### Excel Reports
- **Summary Dashboard**: Cross-stock comparison with key metrics
- **Price Projections**: Statistical breakdown of simulated price paths
- **Return Analysis**: Total and annualized returns with percentile distributions
- **Investment Outcomes**: P&L scenarios based on $10,000 investment per stock
- **Momentum Indicators**: Current technical signal values and interpretations
- **Model Parameters**: Base and adjusted drift/volatility with momentum/macro adjustments

### Professional Visualizations
- **Simulated Price Paths**: 300 sample paths with confidence bands (10th-90th percentiles)
- **Final Price Distribution**: Histogram with current, mean, and median price markers
- **Total Return Distribution**: Percentage return analysis with break-even line
- **Profit/Loss Distribution**: Dollar-based P&L scenarios
- **Momentum Indicator Bar Chart**: Current RSI, MACD, BB position, MA momentum values
- **Risk Metrics Summary**: VaR, CVaR, max loss, mean P&L, upside potential

## Technical Implementation

### Data Processing
- **5-Year Historical Data**: Via Yahoo Finance API for stocks and macro indicators
- **Real-time Price Updates**: Current market prices for position valuation
- **Currency Auto-Detection**: CAD/USD handling for Canadian stocks (.TO tickers)
- **Timezone Handling**: Robust timezone-naive data processing

### Simulation Engine
- **Enhanced GBM Formula**: S(t) = S(t-1) × exp((μ - 0.5σ²)dt + σ√dt × Z + Jumps)
- **Momentum Adjustments**: RSI, BB position, and MA momentum factors
- **Macro Adjustments**: VIX fear factor, interest rate sensitivity, market correlation
- **Jump Diffusion**: Poisson process for rare market events

### Risk Calculation
- **Monte Carlo Statistics**: Mean, median, percentiles across 50,000 paths
- **Investment Analysis**: Share calculations and dollar-based outcomes
- **Probability Metrics**: Profit/loss likelihood calculations

## Technical Stack

- **Python**: NumPy, Pandas, SciPy for numerical computations and statistics
- **Data Sources**: Yahoo Finance API for real-time market data
- **Visualization**: Matplotlib, Seaborn for professional charts
- **Reporting**: Excel integration with xlsxwriter and openpyxl
- **Statistical Analysis**: Monte Carlo simulation, correlation analysis, jump detection

## Use Cases

- Portfolio risk assessment and optimization
- Investment research and due diligence
- Quantitative trading strategy development
- Academic research in financial modeling
- Multi-currency portfolio analysis (CAD/USD)

## Project Status

Active development with continuous improvements to modeling accuracy, additional technical indicators, and machine learning integration planned.
