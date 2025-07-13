# Key Features:
1. GBM with Multiple Factors

Momentum Integration: RSI, MACD, Bollinger Bands, Moving Average convergence
Macroeconomic Factors: VIX (volatility), 10-Year Treasury, S&P 500 correlation, Dollar Index
Jump Diffusion: Detects and models sudden price jumps beyond normal volatility
Dynamic Parameter Adjustment: Drift and volatility adjusted based on current market conditions

2. Advanced Momentum Analysis

RSI (Relative Strength Index): Overbought/oversold conditions
MACD: Trend momentum and signal crossovers
Bollinger Bands: Price position relative to volatility bands
Moving Average Momentum: 50-day vs 200-day MA convergence
Price vs MA: Current price relative to key moving averages

3. Macroeconomic Integration

VIX Correlation: Market fear/volatility sensitivity
Interest Rate Sensitivity: 10-year Treasury correlation
Market Beta: S&P 500 correlation for systematic risk
Dollar Strength: Currency impact on stock performance

4. Jump Diffusion Modeling

Automatic Jump Detection: Identifies returns beyond 3-sigma events
Jump Parameters: Frequency, magnitude, and volatility of jumps
Realistic Price Movements: Captures sudden market shocks and news events

5. Comprehensive Risk Analysis

Value at Risk (VaR): 5% worst-case scenarios
Conditional VaR: Average loss in worst 5% of outcomes
Maximum Drawdown: Worst possible loss
Upside Potential: 95th percentile gains
Profit Probability: Likelihood of positive returns

6. Individual Stock Focus

Per-Stock Analysis: Each stock analyzed independently
Custom Investment Amounts: Flexible investment per stock
Detailed Projections: 2-year forward-looking simulations
50,000 Monte Carlo Paths: High-precision probability estimates

# What the System Outputs:

Excel Report with Multiple Sheets:

Summary Dashboard - All stocks compared side-by-side
Individual Stock Analysis - Detailed breakdown per stock
Price Projections - Statistical analysis of future prices
Return Analysis - Total and annualized return distributions
Investment Outcomes - Profit/loss scenarios
Model Parameters - All technical indicators and adjustments
Momentum Indicators - Current technical analysis signals

Visualizations for Each Stock:

Price Path Simulations with confidence bands
Final Price Distribution histograms
Return Distribution analysis
Profit/Loss Scenarios
Current Momentum Indicators bar charts
Risk Metrics visualization


# How It Works:

Data Collection: Fetches 5 years of historical data plus macroeconomic indicators
Momentum Calculation: Computes all technical indicators for current market state
Correlation Analysis: Determines sensitivity to macro factors
Jump Detection: Identifies historical jump patterns
Parameter Adjustment: Modifies base GBM parameters based on momentum and macro conditions
Monte Carlo Simulation: Runs 50,000 scenarios with enhanced model
Statistical Analysis: Calculates comprehensive risk and return metrics
Visualization: Creates detailed charts for each stock
Report Generation: Produces professional Excel report with all findings
