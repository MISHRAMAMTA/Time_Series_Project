# Time_Series_Project
# ⚡ Time Series Forecasting — U.S. Electric Production

This project is about forecasting monthly **electric production in the United States** using classical time series models.  
I worked on this dataset to understand seasonality, trend, and how different forecasting methods perform over time.

---

## 📊 Dataset
The dataset contains **monthly electric production** data (in million kilowatt-hours) from **1985 to 2018**.  
It’s taken from the **Federal Reserve Economic Data (FRED)** source and has just one main variable, which makes it simple but interesting to work with.

---

## 🚀 Project Overview
Here’s a quick outline of what I did:

### 1️⃣ Data Exploration
- Loaded and cleaned the data using Pandas.  
- Converted the date column properly and checked for missing values.  
- Renamed columns for better readability.

### 2️⃣ Visualization
- Created different time series plots to observe **trend and seasonality**.  
- Used decomposition plots to understand components separately.

### 3️⃣ Stationarity Check
- Used **rolling mean**, **rolling std**, and **ADF test** to check if the data is stationary.  
- Applied differencing (and seasonal differencing) to make it stationary when needed.

### 4️⃣ Modeling
- Tried multiple models:
  - **Exponential Smoothing (Holt-Winters)**
  - **Auto ARIMA**
  - **SARIMA (manually tuned)**
- Compared model results using common error metrics.

### 5️⃣ Model Evaluation
I compared the models using MAE, RMSE, and MAPE.  
The **SARIMA model** performed best with a MAPE around **2.5%**, meaning it captured seasonality and trends quite well.

---

## ✅ Key Insights
- The data shows strong **seasonal patterns**, repeating every year.  
- **Differencing** played a big role in making the data stable.  
- Auto-ARIMA gave a good starting point, but manual tuning helped achieve better accuracy.  
- Visualization really helps in understanding how stable or seasonal the data is.

---

## 🧰 Tools & Libraries
- Python 🐍  
- NumPy, Pandas  
- Matplotlib, Seaborn, Plotly  
- Statsmodels, Pmdarima  
- Scikit-learn

---
