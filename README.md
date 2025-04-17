# 📈 Algorithmic Trading Bot using SVM and Technical Indicators

This project is an **algorithmic trading bot** built with Python 3.9 in **Jupyter Notebook** using real-time market data, technical indicators, and a machine learning model (SVC). It analyzes stock trends and generates **buy/sell signals** based on indicator values and model predictions.

---

## 🔧 Tech Stack

- **IDE**: Visual Studio Code
- **Interpreter**: Jupyter Notebook
- **Language**: Python 3.9

### 📚 Libraries Used

| Category              | Libraries                                     |
|-----------------------|-----------------------------------------------|
| Data Manipulation     | `pandas`, `numpy`                             |
| Visualization         | `plotly`                                      |
| Live Market Data      | `yfinance`                                    |
| Technical Indicators  | `TA-Lib`                                      |
| Machine Learning      | `scikit-learn` – `SVC` (Support Vector Classifier) |

---

## 📦 Setup Instructions

### 1. Install Dependencies

```bash
pip install yfinance pandas numpy plotly ta-lib scikit-learn
🔔 TA-Lib may require additional setup depending on your OS. See: https://mrjbq7.github.io/ta-lib/install.html

2. Run the Notebook
Open the notebook in VS Code or Jupyter Lab:

bash
Copy
Edit
jupyter notebook trading_bot.ipynb
💹 How It Works
Fetch Live Market Data
Using yfinance, the bot pulls historical stock data (e.g., AAPL).

Apply Technical Indicators
Calculates:

RSI (Relative Strength Index)

SMA / EMA (Simple / Exponential Moving Averages)

MACD

Generate Signals
Based on RSI thresholds:

RSI < 30 → Buy

RSI > 70 → Sell

Otherwise → Hold

Machine Learning Prediction

Uses SVC to learn from indicators

Predicts future signals

Visualization
Plots:

Candlestick chart

RSI overlay