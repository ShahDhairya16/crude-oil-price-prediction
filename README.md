# 🚀 Crude Oil Price Prediction using Machine Learning

## 📌 Overview

This project focuses on analyzing historical crude oil prices and building machine learning models to **forecast future prices**.
It combines **time-series feature engineering** (lag and rolling statistics) with regression models to capture short-term market trends.

---

## 🎯 Objective

To predict the **next day’s crude oil price** using historical price data and engineered features.

---

## 📊 Dataset

* Historical crude oil price dataset
* Time-based data (daily prices)

---

## 🔍 Exploratory Data Analysis (EDA)

Key analyses performed:

* Price trend visualization over time
* Weekly and monthly volatility (rolling standard deviation)
* Seasonal patterns (month/year analysis)
* Correlation analysis between features

---

## ⚙️ Feature Engineering

To improve prediction performance, the following features were created:

* **Lag Features**

  * `lag_1`: Previous day price
  * `lag_7`: Price from the previous week

* **Rolling Features**

  * `rolling_mean_7`: 7-day moving average
  * `rolling_std_7`: 7-day volatility

* **Target Variable**

  * `target`: Next day price (`shift(-1)`)

---

## 🤖 Models Used

* Linear Regression
* Random Forest Regressor

---

## 📈 Model Performance

| Model             | MAE   | R² Score |
| ----------------- | ----- | -------- |
| Linear Regression | ~5.17 | ~0.79    |
| Random Forest     | ~7.65 | ~0.54    |

---

## 📊 Visualizations

* Actual vs Predicted price trends
* Error analysis plots
* Distribution of prediction errors
* Feature importance (Random Forest)

---

## 🧠 Key Insights

* Crude oil prices show **strong dependency on previous values**
* Lag features significantly improve prediction accuracy
* Simpler models (Linear Regression) outperform complex ones on small datasets
* Feature engineering plays a critical role in time-series modeling

---

## ⚠️ Challenges

* Limited dataset size (~400 usable rows after preprocessing)
* High correlation between features leading to simpler model dominance
* Handling data leakage during feature creation

---

## 🚀 Future Improvements

* Implement advanced models like XGBoost
* Perform multi-step forecasting (predict multiple future days)
* Incorporate external factors (economic indicators, global events)
* Build an interactive dashboard for real-time predictions

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn, Plotly
* Scikit-learn

---

## 📂 Project Structure

```
crude-oil-price-prediction/
│── data/
│   └── crude-oil-price.csv
│
│── notebook/
│   └── oil_price_analysis.ipynb
│
│── README.md
│── requirements.txt
```

---

## 📌 Conclusion

This project demonstrates how time-series feature engineering combined with machine learning can effectively model short-term crude oil price movements.
While results are promising, further improvements can be achieved with more data and advanced modeling techniques.

---

## 👨‍💻 Author

Dhairya Shah

---

## ⭐ If you found this useful, consider giving this repository a star!
