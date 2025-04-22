# Quantum Strategy 📈  
A math and statistics-based BTC/USDT trading strategy designed for directional signal generation and ATR-based risk management.  
This signal system is intended as a **reference for long/short trading decisions** and is under active development.

## 📌 Features
- Directional Score System (long/short)
- 2× ATR Take-Profit, 1× ATR Stop-Loss
- Score ≥ 1 triggers a trade
- Leverage: 5× simulated
- Backtest ROI: Currently ongoing using historical BTCUSDT data from 2021–2024  
  Preliminary results show stable signal reliability across multiple market phases.
> ⚠️ This strategy provides **signal-based guidance** and does **not** incorporate news events, liquidation maps, funding rates, or market sentiment (FOMO). Use it with discretion and alongside other tools.
>
> ## 🔭 Strategy Use & Future Direction
This strategy serves as a **signal indicator for discretionary long/short trading**.  
Over the next year, it will undergo **live forward-testing**, with the goal of evolving into an **automated trading bot** integrated with exchange APIs.

The vision:
- 🔁 Automate trade execution using live data
- 🔌 Connect to Binance and other exchange APIs
- 🔄 Support real-time signal updates and logging
- 📈 Monitor and visualize PnL, win rate, drawdown, etc.
  
---

## 📊 Strategy Logic Summary

| Component                  | Description |
|---------------------------|-------------|
| 📈 **Directional Score**   | Aggregates RSI, EMA structure, pattern match signals with weighted scoring |
| 📉 **ATR-based Risk Control** | Uses dynamic market volatility to determine TP/SL levels |
| 🧠 **Why scoring system?** | Enables reproducibility and probabilistic edge from multi-signal convergence |
| 🧠 **Why ATR?**            | Adapts to changing volatility; avoids overfitting fixed SL/TP settings |

---

## 📸 Signal Snapshot Example  
*Long: Green (L3+), Short: Red (S-2, S-3)*  
*(BTCUSDT Perpetual, BINANCE – 5m, 30m, 1h)*

### 🕔 5-minute Chart
![5m](images/QS%205min.png)

### 🕧 30-minute Chart
![30m](images/QS%2030m.png)

### 🕐 1-hour Chart
![1h](images/QS%201h.png)



---

## 🧪 Files
- `quantum_strategy_v1.py`: Core score and ATR logic
- `backtest/`: Historical performance & logs
- `config/settings.json`: Parameter config

---

## 🛠️ Setup
> Coming soon:  
> - Install instructions  
> - Pine Script deployment  
> - Backtesting guide with TradingView + Python script

---

## 🚀 Roadmap
- Incorporate liquidation map data (Binance/Bubble Charts)
- Real-time funding rate trend tracking
- Add sentiment filters via Twitter sentiment APIs
- Multi-algo framework with regime detection
- Machine-learning scoring model for L/S prediction

---

## 📬 Contact

> Strategy developed by **Kiin Chang**  
> For collaboration or integration inquiries:  
📧 **wedo101@gmail.com**

---

## 🔐 Note

> ⚠️ The **full Pine Script code is not open-source**.  
> The public version shares performance snapshots and key logic.  
> If you're interested in collaboration or licensing, please reach out.

---


