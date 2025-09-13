# 📊 Portfolio Optimization & Risk Management  

This project applies **Modern Portfolio Theory (MPT)** to optimize a portfolio of trending technology assets from 2019–2025.  
It explores stock performance, risk–return trade-offs, and portfolio construction using **Monte Carlo simulation, Efficient Frontier optimization, and downside risk metrics**.  

---

## 🚀 Project Overview  
Investors face a trade-off between **risk** (volatility) and **return** (growth).  
This project demonstrates how to:  

- 📈 Collect and analyze stock market data  
- 🔍 Explore asset behavior (returns, volatility, correlations)  
- 🎲 Simulate thousands of random portfolios (Monte Carlo)  
- 📊 Identify optimal portfolios (Max Sharpe & Min Volatility)  
- 📉 Evaluate downside risk (VaR, CVaR, Max Drawdown)  

---

---

## 🛠️ Tech Stack  

- **Python**: pandas, numpy, matplotlib, seaborn, scipy  
- **Finance**: Modern Portfolio Theory (Markowitz), Sharpe Ratio, Risk Measures  
- **Optimization**: scipy.optimize for Efficient Frontier  
- **Visualization**: cumulative returns, risk-return scatterplots, correlation heatmap  

---

## 📈 Analysis Steps  

### 1. Exploratory Data Analysis (EDA)  
- Assets: **AAPL, AMZN, GOOGL, META, MSFT, NVDA, TSLA**  
- Visualized stock price trends & cumulative returns  
- Calculated annualized returns, volatility, and correlations  

📊 *Key Finding*:  
- NVDA and TSLA → explosive growth but high volatility  
- AAPL and MSFT → stable compounders  
- AMZN and GOOGL → reliable giants  
- META → cyclical and opportunistic  

---

### 2. Monte Carlo Portfolio Simulation  
- Generated **100,000 random portfolios**  
- Calculated return, volatility, and Sharpe ratio  
- Plotted portfolios in risk–return space  

📊 *Key Finding*: Portfolios form a “cloud” — the **upper edge is the Efficient Frontier**.  

---

### 3. Efficient Frontier Optimization (NumPy + SciPy)  
- Identified **Maximum Sharpe Ratio Portfolio** (best risk-adjusted return)  
- Identified **Minimum Volatility Portfolio**  
- Plotted the Efficient Frontier curve  

📊 *Key Finding*: Investors can select along the frontier based on risk tolerance.  

---

### 4. Downside Risk Analysis  
- Computed **Value at Risk (VaR)**, **Conditional VaR (CVaR)**, and **Maximum Drawdown**  

📊 *Results (Max Sharpe Portfolio)*:  
- 95% VaR: -4.2%  
- 95% CVaR: -6.0%  
- Maximum Drawdown: -53.8%  

👉 Even the “optimal” portfolio can suffer severe losses during downturns.  

---

## ✅ Conclusion & Recommendations  

- **Diversification matters**: combining stable stocks (AAPL, MSFT) with high-growth bets (TSLA, NVDA) balances performance and risk  
- **Efficient Frontier helps** align portfolios with risk tolerance  
- **Downside risk is critical**: averages hide extreme losses  

**Example Balanced Allocation Strategy**:  
- 40% AAPL + MSFT (anchors)  
- 30% NVDA + TSLA (growth)  
- 20% AMZN + GOOGL (defensive)  
- 10% META (opportunistic)  

---

## 📌 Future Work  
- Extend analysis to ETFs, bonds, or commodities  
- Add dynamic rebalancing strategies  
- Build an interactive **Streamlit dashboard**  

---

