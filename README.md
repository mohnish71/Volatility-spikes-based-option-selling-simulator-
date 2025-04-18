# Volatility-spikes-based-option-selling-simulator-

Simulating a volatility spike options strategy (~400 trades) using Black-scholes, with 50%+ win rate; adding risk controls and live backtesting.

Overview 

This project simulates an options trading strategy based on volatility spikes detected in US stocks (e.g., TSLA, NVDA).
It sells ATM call options during high volatility periods and closes the position after 7 days, aiming to capture volatility mean reversion.

Highlights

1. Detected volatility spikes using 30-day Historical Volatility (HV) exceeding 1.2× its moving average.

2. Modeled option prices using the Black-Scholes formula assuming pricing to be theoritical, 

3. Simulated over 209 trades (TSLA) and 215 trades (NVDA) from 2018–2024.

4. Achieved ~52% win rate across stocks, validating the hypothesis of mean reversion post-volatility spikes.

Tech Stack : Python, Pandas, NumPy, Matplotlib, Yahoo Finance API (yfinance), SciPy (Black-Scholes pricing)

Work in Progress :

1. Adding risk management modules (stop-loss, dynamic exits).

2. Integrating put options for straddle/strangle strategies.

3. Setting up live data collection for better backtesting and future paper trading.
   

Required libraries : numpy, pandas, matplotlib, yfinance and scipy. 

More improvements and live trading modules coming soon!
