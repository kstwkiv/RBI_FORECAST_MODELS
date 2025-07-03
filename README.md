# RBI_FORECAST_MODELS

##  Project Description

**Title**: RBI Investment Forecasting Using ARIMA vs XGBoost
**Domain**: FinTech · Time-Series Forecasting · Data Science

###  Overview:

This project analyzes and forecasts **RBI’s Scheduled Commercial Banks' investments in SLR Securities** using two distinct time-series modeling approaches:

* **ARIMA (AutoRegressive Integrated Moving Average)** — a statistical forecasting model
* **XGBoost (Extreme Gradient Boosting)** — a powerful machine learning model

My objective is to compare both models' performance on real RBI financial data, focusing on forecast accuracy and model interpretability.

---

###  Dataset:

The data comes from RBI’s public financial bulletins, containing fortnightly figures for various investment categories by commercial banks — specifically:

* **1 SLR Securities**
* **Other government securities, bonds, commercial papers**, etc.

The data was cleaned from an unstructured Excel format using `pandas` and reshaped into a time-series format indexed by date.

---

###  Models Used:

* **ARIMA**: Captures trends and autocorrelation directly from the time series. Suitable for sequential data with minimal feature engineering.
* **XGBoost**: Used with lag-based features to predict future values. Powerful but sensitive to feature design in time series.

---

###  Evaluation:

Models were evaluated using **Root Mean Squared Error (RMSE)** on a held-out test set.

| Model   | RMSE        |
| ------- | ----------- |
| ARIMA   | ₹33,185.76  |
| XGBoost | ₹222,147.12 |

**Conclusion**:
ARIMA significantly outperformed XGBoost for this dataset, making it a more suitable choice for forecasting structured financial time-series data like RBI investments.

---

###  Key Highlights:

* Real-world RBI financial dataset
* Full data cleaning, transformation, and visualization pipeline
* Dual model training: classical stats vs modern ML
* Forecast plots and RMSE-based comparison
* Notebook-ready and deployable via Streamlit

---

