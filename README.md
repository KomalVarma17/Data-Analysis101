# 📊 Retail Sales Forecast Accuracy & Revenue Drivers

This project analyzes retail sales data to measure **forecast accuracy**, understand the **impact of product returns**, and connect **order quantity trends** to overall revenue performance. The final deliverable is a clear, interactive Tableau dashboard designed for real-world business decision-making.

---

## 🚀 Project Objective


Retailers lose significant revenue due to poor forecast accuracy and unmanaged product returns. This project helps bridge the gap between actual sales, forecast models, and order trends to improve planning and reduce revenue leakage.
 
- Compare actual gross and net revenue with **ARIMA**, **Prophet**, and **Regression** forecast models.
- Visualize the financial impact of returns on net revenue.
- Link monthly order quantity trends to sales performance.

---


---

## 🧩 Key Steps

### 1️⃣ Data Preparation
- Cleaned raw transaction data, handled missing Customer IDs, removed large outliers and flagged canceled orders.
- Engineered new metrics: Gross Revenue, Returns, Net Revenue.
- Aggregated revenue by month for time series forecasting.

### 2️⃣ Forecast Modeling
- Built **ARIMA** and **SARIMA** models to test autocorrelation.
- Applied **Prophet** for robust trend and seasonality detection.
- Built baseline **Regression** models, including Regression with month dummies.
- Evaluated performance using **MAE** and **RMSE** metrics.

### 3️⃣ Dashboard in Tableau
- Designed an interactive Tableau dashboard with:
  - *Gross vs Net Revenue & Forecasts*
  - *Returns Impact*
  - *Monthly Net Revenue vs Quantity Ordered*
  - *Forecast Accuracy KPIs*
- Added clean legends, color consistency, and interactive date filters.

---

## 🔍 Key Insights

- **Prophet outperformed ARIMA and Regression**, achieving the lowest MAE and RMSE.
- Certain countries (e.g., Singapore, USA) showed >50% return rates, significantly affecting net revenue.
- 90% of orders were small (quantities under 10), but large bulk returns distorted total revenue.
- December showed the highest forecast deviation due to seasonal sales spikes.

---

## 📊 Tools Used

- **Python:** Pandas, Statsmodels (ARIMA), Prophet, Scikit-learn (Regression)
- **Tableau:** Dashboard design, interactive charts, KPIs, filters
- **Version Control:** Git & GitHub for code and files

---

## ✅ Final Deliverable

- 📈 Fully interactive Tableau dashboard with real business storytelling.
- Clear insights on actual vs forecast revenue, returns impact, and order trends.
- Export-ready for presentations or reporting.

---

## 🔗 Live Dashboard

👉 [**View the Published Tableau Dashboard Here**](https://public.tableau.com/app/profile/komal.penmatsa/viz/Book2_17518731668780/Dashboard2)

---

## 📈 Forecast Accuracy

| Model               | MAE           | RMSE          |
|---------------------|----------------|----------------|
| ARIMA               | 517,485.78     | 638,683.22     |
| **Prophet**             | **21,673.41**  | **25,196.17**  |
| Regression w/ Month | 833,244.33     | 1,011,483.76   |

---

## ⚡️ Next Steps

- Add more historical data to strengthen time series performance.
- Automate data updates and forecasting for monthly reporting.
- Expand to a Power BI version for wider deployment.

---

**If you find this helpful, please ⭐️ star the repo or connect for collaboration!**
