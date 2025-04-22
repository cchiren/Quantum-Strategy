# Quantum Strategy 📈  
A scientific BTC/USDT trading strategy using directional scoring and ATR-based TP/SL.

## 📌 Features
- Directional Score System (long/short)
- 2× ATR Take-Profit, 1× ATR Stop-Loss
- Score ≥ 1 triggers a trade
- Leverage: 5× simulated
- Backtest ROI: Backtest is currently in progress using historical BTCUSDT data from 2021–2024.  
Preliminary results show promising signal reliability and risk-reward balance under multiple market conditions.

> ⚠️ Final ROI metrics will be shared after validation and optimization.

> ⚠️ This indicator provides **signal-based guidance** for discretionary trading.  
> It **does not account for** news events, liquidation heatmaps, funding rate trends, or market sentiment (FOMO).  
> Use with caution and **combine with other tools**.

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
- `quantum_strategy_v1.py` – Core Pine Script logic
- `backtest/` – Backtesting CSVs and summaries
- `config/settings.json` – Strategy parameters and weight coefficients

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


