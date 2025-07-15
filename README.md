
# 📈 Nifty-50 Price Prediction using XGBoost Classifier

This project uses **XGBoost (Extreme Gradient Boosting)** to build a classification model for **predicting the price movement (Up/Down)** of **Nifty-50 stocks** based on historical data and technical indicators.

---

## 🚀 Overview

Nifty-50 is a benchmark stock market index representing the weighted average of 50 of the largest Indian companies listed on the NSE. Accurately predicting its movement can assist traders and analysts in making better decisions.

In this project, we:
- Collected and preprocessed historical stock price data
- Engineered features like moving averages, RSI, and MACD
- Built and trained an XGBoost Classifier
- Evaluated performance using metrics like Accuracy, Precision, Recall, F1 Score, and ROC AUC
- Visualized feature importance and model evaluation curves

---

## 📊 Features Used

- **Open, High, Low, Close, Volume**
- **Technical Indicators**:
  - 10-day, 20-day, and 50-day moving averages (SMA/EMA)
  - RSI (Relative Strength Index)
  - MACD (Moving Average Convergence Divergence)
  - Bollinger Bands
  - Price Momentum
- **Target Label**: `1` for **Upward Movement**, `0` for **Downward Movement**

---

## 🛠️ Tools & Libraries

- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- **xgboost**
- TA-Lib (for technical indicators) *(optional)*

---

## 📁 Project Structure

```

nifty-50-xgboost/
├── nifty50\_xgb\_classifier.ipynb       # Main notebook
├── model.pkl                          # Saved XGBoost model
├── data/
│   └── nifty50\_data.csv               # Historical price data
├── plots/
│   ├── roc\_curve.png
│   └── feature\_importance.png
├── README.md
└── requirements.txt
you can make this way....
````

---

## 📈 Model Performance

| Metric          | Score     |
|-----------------|-----------|
| Accuracy        | 50.36%    |
| Precision       | 50.38%    |
| Recall          | 98.85%    |
| F1 Score        | 66.75%    |
| ROC AUC         | 50.16%    |

> ⚠️ High recall but low precision and AUC indicate the model may be biased toward predicting upward movements. Further feature tuning and class balancing are needed.

---

## 📌 How to Run

1. Clone the repo:
```bash
git clone https://github.com/your-username/nifty-50-xgboost.git
cd nifty-50-xgboost
````

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the notebook:

```bash
jupyter notebook nifty-50.ipynb
```

---

## ✅ Future Improvements

* Improve feature engineering (e.g., sector-wise indicators)
* Try ensemble models (Random Forest, LSTM)
* Optimize with GridSearchCV or Optuna
* Add backtesting for real-world trading simulation

---

## 📬 Contact

* **Author**: Charan B
---

## ⭐ Give a star!

If you found this project useful, feel free to ⭐ the repo!

````

---

### ✅ Optional Files:

**`requirements.txt`**
```txt
xgboost
pandas
numpy
scikit-learn
matplotlib
seaborn
````

