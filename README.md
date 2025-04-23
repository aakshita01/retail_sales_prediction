# 🛒 Retail Sales Forecasting Using Time Series Models

Predict future retail sales using historical monthly sales data. Initial attempts using ML models showed poor performance due to the time-dependent nature of the data, prompting a shift to time series forecasting techniques.

---

## 📁 Project Structure

```
RETAIL_SALES_PREDICTION/
├── data/
│   ├── Train.csv
|   ├── Events_HolidaysData.xlsx
|   ├── MacroEconomicData.xlsx
|   └──  WeatherData.xlsx
├── notebooks/
│   ├── retail_sales_prediction.ipynb         # ML-based forecasting models
│   └── timeseries_data_visualization.ipynb   # Time series EDA + visualization
├── requirements.txt
└── README.md
```
---

## 🧠 Models Applied

### 🕒 Time Series Forecasting Models:
| Model            | MAE     | MAPE    |
|------------------|---------|---------|
| **SARIMAX**      | 139.81  | **7.89%** ✅ Best performing model
| Holt-Winters     | 151.83  | 8.37%   |
| Prophet          | 160.64  | 8.68%   |
| ARIMA            | 242.65  | 14.03%  |
| Weighted MA      | 250.87  | 12.61%  |
| Simple MA        | 308.50  | 14.76%  |

### ⚙️ Machine Learning Models:
| Model            | MAE     | MAPE    |
|------------------|---------|---------|
| XGBoost          | 345.53  | 21.73%  |
| Random Forest    | 339.49  | 21.03%  |
| Linear Regression| 562.07  | 41.12%  |
| SVR              | 977.30  | 53.32%  |

---

## 🔧 How to Run

1. Clone the repo
```bash
git clone https://github.com/your-username/retail-sales-forecasting.git
cd retail-sales-forecasting
```

2. Create virtual environment & install dependencies
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook
```bash
jupyter notebook
```

4. Run the notebooks:
- `retail_sales_prediction.ipynb`
- `timeseries_data_visualization.ipynb`

---
## 🔍 Insights
- ML models underperformed due to lack of temporal feature engineering (lags, trend, seasonality)
- Time series models captured seasonal patterns better
- SARIMAX showed strongest performance in both error metrics and visual alignment

## 📈 Visualizations
- Rolling Mean & Std Deviation checks for stationarity
- Prophet and SARIMAX forecast confidence intervals
- MA/EMA/WMA overlays on sales

## ✅ Key Takeaway
Time series models are far more suited than traditional ML models for forecasting problems where data is highly seasonal and trend-based. This project clearly demonstrates the superiority of SARIMAX over other forecasting techniques.

---

## 📦 Requirements
See [`requirements.txt`](./requirements.txt)

---

## 📧 Contact
Akshita Aluru — [LinkedIn](https://linkedin.com/in/akshita-aluru-7664a1217)

