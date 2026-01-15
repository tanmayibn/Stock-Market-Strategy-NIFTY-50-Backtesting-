# Stock-Market-Strategy-NIFTY-50-Backtesting-


# Trinetra 2.0 – Long Only Trading Strategy

##  Introduction

Trinetra 2.0 is a **trend-following, long-only trading strategy** built in Pine Script v5 for TradingView.
The idea behind this system is simple:

* Use **Heikin Ashi candles** to reduce noise
* Combine **dual EMAs (21 & 55)** to confirm market direction
* Deploy an **ATR-based trailing stop** to dynamically manage risk

The focus of this project is not just to generate signals, but to create a **robust trading framework** that adapts to volatility and provides steady growth over time.


## Key Highlights

*  **Heikin Ashi Filtering** → Smoothens price action and avoids false signals
*  **Dual EMA Confirmation** (21 EMA & 55 EMA) → Captures medium-term trend direction
*  **ATR-based Trailing Stop** → Automatically adjusts stop loss based on volatility
*  **Long-Only Logic** → Focused on capturing upside moves
*  **Fixed Position Size** (default: 100 quantity, can be adjusted)



## Backtesting Performance

The strategy was tested on a **2-hour timeframe** from **Jan 2020 to Sep 2025**.
Below are the key results:

* **Total Net Profit:** +₹22,81,935 (≈ +228.19%)
* **Profit Factor:** 16.87 (very strong risk-reward balance)
* **Max Drawdown:** 3.07% (extremely low risk exposure)
* **Total Trades:** 126
* **Win Rate:** 72.22% (91 out of 126 trades profitable)

 In simple terms, this means the system was able to grow equity consistently while keeping drawdowns small — an important aspect of real-world trading.





##  Strategy Logic – How It Works

1. **Entry Condition:**

   * Heikin Ashi close crosses **above** the trailing stop
   * 21 EMA is greater than 55 EMA (bullish trend confirmation)

2. **Exit Condition:**

   * Heikin Ashi close crosses **below** the trailing stop

3. **Trailing Stop Mechanism:**

   * The stop is calculated using **ATR × multiplier**
   * Adjusts dynamically based on volatility
   * Protects profits when the price moves in favor



##  How to Use the Strategy

1. Open TradingView and go to the **Pine Editor**
2. Copy-paste the script and **add to chart**
3. Recommended timeframe → **2H** (optimized for this setup)
4. Use the **Strategy Tester** to analyze performance or customize parameters (EMA length, ATR multiplier, etc.)



##  Important Notes

* This is a **backtested strategy**. Past performance does not guarantee future results.
* It is designed for **educational and research purposes only**.
* Always perform **paper trading** before applying it to live markets.
* Consider combining it with broader market analysis, position sizing, and risk management techniques.



##  Closing Thoughts

Trinetra 2.0 is my attempt to design a clean, rules-based trading system that emphasizes:

* Simplicity in logic
* Robust risk management
* Steady equity curve with low drawdowns


Would you like me to **add a “Quick Start” code section** (with installation steps + example snippet) so people on GitHub can immediately run your script?
