# 📊 Project 1: Regime-Switching Portfolio Optimization

This project applies a Hidden Markov Model (HMM) to financial return data to detect distinct **market regimes** (such as bull, bear, and neutral markets). The goal is to build a dynamic portfolio strategy that adapts asset allocation based on these regimes.

---

## 🗂️ Project Structure

Project1_RegimeSwitching/
├── data/ # Raw and processed data files (e.g., prices.csv, returns.csv)
├── notebooks/ # Week-by-week development notebooks
├── figures/ # Plots for presentation or report
├── README.md # You're reading it!
├── requirements.txt# Python packages used in the project

---

## ✅ Progress by Week

### Week 1: Data Collection & Preprocessing
- Downloaded adjusted closing prices for SPY, TLT, and GLD
- Calculated daily log returns
- Cleaned and visualized the time series
- Saved data to `/data` for modeling

### Week 2: Regime Detection with HMM *(in progress)*
- Use `hmmlearn` to classify time periods into market regimes

### Week 3: Strategy Simulation *(planned)*
- Allocate weights differently per regime
- Backtest against a static 60/40 portfolio

### Week 4: Final Report & Analysis *(planned)*
- Evaluate Sharpe, drawdown, switching frequency
- Wrap into presentation-ready results

---

## 📌 Tools Used

- Python 3.11
- Jupyter Notebook
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `yfinance` (for financial data)
- `hmmlearn` (for Hidden Markov Models)

---

## 💡 Future Ideas
- Extend to more assets or macro indicators
- Add forecasting logic (next-step regime probabilities)
- Build a Dash or Streamlit dashboard for live visualization

---

## 🧠 Author Notes

This project is part of my personal quant learning journey. It's structured to reflect how a quant research team might break down, build, and backtest a strategy based on observable regime changes.

