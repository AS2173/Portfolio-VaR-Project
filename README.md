# Portfolio VaR Project

This project estimates the 1-day downside risk of a £100,000 multi-asset portfolio using Python.

## Portfolio
The portfolio consists of:
- SPY
- GLD
- TLT
- USO

Portfolio weights:
- 40% SPY
- 20% GLD
- 20% TLT
- 20% USO

## Methods Used
- Historical Simulation VaR
- Parametric VaR
- Monte Carlo VaR
- Historical Expected Shortfall (ES)

## Key Results
### 95% VaR
- Historical VaR: £1099.61
- Parametric VaR: £1192.66
- Monte Carlo VaR: £1200.24

### 99% VaR
- Historical VaR: £1974.66
- Parametric VaR: £1709.14
- Monte Carlo VaR: £1704.74

### Historical Expected Shortfall
- 95% ES: £1681.30
- 99% ES: £2457.62

## Main Insight
Parametric VaR and Monte Carlo VaR produced very similar estimates because the Monte Carlo simulation was based on a normal distribution using the portfolio mean and standard deviation. Historical VaR was higher at the 99% confidence level, suggesting that the empirical return distribution contains more severe tail losses than a simple normal model captures.

## File
- `Portfolio_VaR_Project.ipynb` — full notebook containing the analysis, charts, and interpretations
