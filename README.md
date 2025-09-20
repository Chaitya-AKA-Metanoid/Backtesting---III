# Backtesting---III
Absolutely 👍 — let’s make your README more **visual and reader-friendly**, while still keeping that diary-style “I tested this today” tone. We can use **emoji, headers, lists, and maybe even an ASCII-style preview** so it feels more alive. Here’s an upgraded draft:

---

# 📈 RSI 30-70 Backtest on NSEI

Hey 👋

Today I decided to test one of the most popular *mean reversion* strategies — the **RSI 30/70 rule** — on **NSEI (Nifty 50) stocks in India**.

The idea is simple:

* ⬇️ **RSI < 30** → stock is oversold → go **long**
* ⬆️ **RSI > 70** → stock is overbought → time to **exit** (or short if you’re brave)

But the real question: *does this actually work in our markets?* 🤔

---

## 🔧 What I Did

✔️ Pulled historical stock data using `yfinance`
✔️ Calculated RSI (no TA-Lib, just pure pandas & numpy)
✔️ Marked **entry/exit points** based on RSI thresholds
✔️ Added a simple **stop-loss** to keep it realistic
✔️ Backtested performance with a starting capital
✔️ Plotted everything with Plotly (interactive charts 🖼️)

---

## 📒 What’s Inside

* `RSI 30-70.ipynb` → the main notebook

  * `calculate_rsi()` → compute RSI
  * `create_trading_signals()` → generate buy/sell signals
  * `backtest_strategy()` → run the capital backtest
  * `plot_rsi_trades()` → interactive visualization

---

## 👀 What You’ll See

* 📊 **Price + RSI Chart** with entry (🟢) and exit (🔴) markers
* 📝 **Trade Log** with entry/exit price, profit/loss, % returns
* 💰 **Capital Curve** to track growth of portfolio

Example (mock view):

```
Trade  | Entry | Exit | P/L%
-----------------------------
Long   | 17150 | 17420 | +1.58%
Long   | 16800 | 16500 | -1.79% (Stop Loss)
```

---

## 🚀 How to Run

```bash
git clone <this-repo>
cd RSI-30-70
pip install pandas numpy yfinance plotly
jupyter notebook RSI\ 30-70.ipynb
```

Run cells top-to-bottom and you’ll see the signals, backtest stats, and charts.

---

## 💡 Why I’m Sharing This

I wanted to test whether this “textbook” RSI strategy actually works for Indian stocks. Spoiler: 📉➡️📈 it’s not a guaranteed money-maker, but it’s a fantastic way to learn about:

* Backtesting 🧪
* Risk management ⚖️
* Where simple strategies fail (and how to improve them)

---

## ⚠️ Disclaimer

This is **not financial advice**. I’m just experimenting and sharing my trading diary with you.

---

