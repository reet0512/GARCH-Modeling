# Delta Hedging Performance in Volatility Regimes

This project investigates how delta hedging frequency impacts hedging effectiveness across different volatility regimes, using both simulated data (GARCH(1,1)) and historical market data (Russell 2000). We explore the tradeoffs between hedge accuracy, transaction costs, and profitability using risk-adjusted metrics such as Sharpe Ratio and Hedge MSE.

## 📈 Project Goals

- Evaluate delta hedging performance under constant and stochastic volatility
- Quantify the impact of hedging frequency on portfolio stability and risk
- Incorporate transaction costs to assess real-world hedging efficiency
- Use Monte Carlo simulations and kernel density estimation for robustness

## 🧠 Key Findings

- **Adaptive hedging strategies** that adjust frequency based on volatility regimes generally outperform static strategies.
- **Excessive hedging** in high-volatility environments may increase error due to transaction costs and gamma exposure.
- **Tradeoffs exist** between hedge precision and cost—no universally optimal strategy.

## 🛠️ Methodology

- Simulated 252-day trading periods with GARCH(1,1) volatility models
- Evaluated hedging strategies at multiple rebalancing intervals (1, 10, 50, 100)
- Computed Sharpe Ratio and Hedge MSE to compare strategies
- Ran 100+ Monte Carlo simulations to visualize hedge error distributions
- Conducted historical analysis using Russell 2000 index options (Nov 2022 – Jan 2023)

## 📊 Tools & Libraries

- Python (NumPy, pandas, matplotlib, SciPy)
- Yahoo Finance and WRDS for option pricing

## 🔍 Future Work

- Test on individual stocks and illiquid options
- Explore alternative volatility models (e.g., EGARCH)
- Introduce order book-based execution to refine transaction cost modeling