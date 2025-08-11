# Project 1: Regime-Switching Portfolio Optimization

This project explores how Hidden Markov Models (HMMs) can be used to detect different market conditions — such as calm bull markets, volatile bear markets, or something in between.  
The idea is simple: if markets behave differently in different regimes, portfolio allocations can adapt to those conditions.

## Project Structure

├── README.md
├── data
│   ├── returns.csv
│   └── returns_with_regimes.csv
├── figures
│   └── phase2_spy_regimes.png
├── notebooks
│   ├── archive.ipynb
│   ├── phase1_data_preparation.ipynb
│   ├── phase2_modeling.ipynb
│   └── phase3_portfolio_backtest.ipynb
└── requirements.txt

## Progress So Far

**Phase 1 – Data Collection & Preprocessing (8/3/2025)**
- Pulled adjusted close prices for SPY, TLT, and GLD using `yfinance`
- Calculated daily log returns
- Performed quick visual checks that data looks valid
- Saved clean data to `/data` for later use

**Phase 2 – Regime Detection with HMM (8/7/2025)**
- Trained a 3-state Gaussian HMM on SPY returns using `hmmlearn`
- Classified each trading day into one of three regimes
- Saved labeled returns and a plot showing SPY returns color-coded by regime

**Phase 3 – Strategy Simulation (8/10/2025)**  
- Assign different portfolio weights depending on the current regime.  
- Compare performance against a 60/40 benchmark portfolio.  

## Next Steps

**Phase 4 – Final Analysis (planned)**  
- Evaluate Sharpe ratio, drawdowns, and regime switching frequency.  
- Package results into a clear, presentation-ready format.

## Tools and Libraries

- Python 3.11  
- Jupyter Notebook, VS Code  
- `pandas`, `numpy`, `matplotlib`, `seaborn`  
- `yfinance` for market data  
- `hmmlearn` for Hidden Markov Models  

## Future Enhancements
- Incorporate additional assets or macroeconomic indicators.
- Include regime-probability forecasts instead of only hard classifications.
- Build a Streamlit or Dash app for interactive visualization.

## Author Notes
I’m approaching this as more than just an HMM experiment — the aim is to practice the same workflow a quant researcher might follow: breaking the project into phases, keeping code and data organized, and tracking changes with version control.  
This is essentially a test run — a way to build my skills and refine my process before tackling a more complex, results-driven project.