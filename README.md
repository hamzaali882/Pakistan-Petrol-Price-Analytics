# 🇵🇰 Pakistan Petrol Price Analytics & Forecasting

## 📌 Project Overview

This project analyzes and forecasts **petrol price changes in Pakistan** using historical petrol prices and key external economic factors, particularly **Brent crude oil prices** and the **USD/PKR exchange rate**.

The project combines exploratory data analysis, correlation analysis, lag analysis, regression modeling, forecasting, model evaluation, and scenario analysis to understand the factors associated with changes in petrol prices.

The goal is to demonstrate how Python and statistical modeling can be used to analyze real-world economic data and generate data-driven insights.

---

## 🎯 Objectives

* Analyze historical petrol price movements in Pakistan.
* Examine the relationship between petrol prices and Brent crude oil prices.
* Investigate the relationship between petrol prices and the USD/PKR exchange rate.
* Identify potential lagged effects of external economic variables.
* Develop regression models to explain changes in petrol prices.
* Build a forecasting model using lagged economic variables.
* Compare actual and predicted petrol price changes and prices.
* Perform scenario analysis to examine potential petrol price movements.

---

## 🛠️ Tools & Technologies

* **Python**
* **Jupyter Notebook**
* **Pandas** — Data manipulation and analysis
* **NumPy** — Numerical computations
* **Matplotlib** — Data visualization
* **Seaborn** — Statistical visualization
* **Statsmodels** — Statistical and regression modeling
* **yfinance** — Financial market data
* **Requests** — Data collection
* **OpenPyXL** — Excel file handling

---

## 📊 Analysis Performed

### 1. Exploratory Data Analysis

The project begins with an examination of the available data to understand its structure and characteristics.

The analysis includes:

* Dataset dimensions and structure
* Column inspection
* Missing-value analysis
* Descriptive statistics
* Historical petrol price analysis

---

### 2. Correlation Analysis

Correlation analysis was performed to examine relationships between petrol prices and relevant economic variables.

A correlation heatmap was created to visualize relationships among numerical variables and identify potentially important predictors.

---

### 3. Petrol Price vs. Brent Crude Oil

Brent crude oil prices were analyzed as an important external factor affecting petrol prices.

The analysis examines:

* Relationship between petrol prices and Brent crude oil
* Correlation between the variables
* Lagged effects of Brent crude oil prices

Both one-period and two-period lag relationships were investigated.

---

### 4. Petrol Price vs. USD/PKR

The USD/PKR exchange rate was also examined because exchange-rate movements can affect the domestic cost of imported petroleum products.

The project analyzes:

* Petrol price vs. USD/PKR
* Correlation between the variables
* Lagged USD/PKR relationships

---

### 5. Lag Analysis

Lag analysis was conducted to determine whether changes in Brent crude oil prices and USD/PKR could be associated with petrol price changes in subsequent periods.

The analysis includes:

* Brent lag correlations
* USD/PKR lag correlations
* Monthly percentage-change correlations
* Lagged monthly change correlations

This helps investigate whether external economic changes may influence petrol prices with a delay rather than immediately.

---

## 📈 Predictive Modeling

Ordinary Least Squares (**OLS**) regression was used to model changes in Pakistan petrol prices.

The forecasting model uses the following predictors:

* **Brent crude oil price — 1-period lag**
* **Brent crude oil price — 2-period lag**
* **USD/PKR exchange rate — 1-period lag**

The dependent variable is:

* **Petrol price change**

The model was trained using a separate training dataset and subsequently evaluated over a test period.

---

## 📊 Model Performance

Several regression specifications were developed during the analysis.

| Model                              |        R² | Adjusted R² |
| ---------------------------------- | --------: | ----------: |
| Initial Regression                 |     0.321 |       0.315 |
| Improved Regression                |     0.352 |       0.344 |
| **Forecast Model — Training Data** | **0.370** |   **0.360** |
| Scenario Model                     |     0.352 |       0.343 |

### Key Result

The final forecasting model achieved an **R² of 0.370** and an **adjusted R² of 0.360** on the training data.

This means the model explains approximately **37.0% of the variation in petrol price changes within the training sample**.

The improved model also increased R² from **0.321 to 0.352** after incorporating an additional Brent crude oil lag, indicating improved explanatory power.

> **Note:** R² represents explanatory power and should not be interpreted as model accuracy.

---

## 🔎 Key Regression Findings

The forecasting model produced the following statistically significant relationships:

* **Brent lag 1:** Positive and statistically significant
* **Brent lag 2:** Positive and statistically significant
* **USD/PKR lag 1:** Positive and statistically significant

The forecast model produced a **Durbin-Watson statistic of 2.074**, indicating limited evidence of first-order autocorrelation in the training residuals.

Overall, the regression results suggest that lagged movements in **Brent crude oil prices** and the **USD/PKR exchange rate** provide useful explanatory information for changes in Pakistan petrol prices.

---

## 🔮 Forecast Evaluation

The forecasting stage compares model predictions with actual observations over the test period.

The project includes visualizations showing:

* Actual vs. predicted petrol price changes
* Actual vs. predicted changes during the test period
* Actual vs. predicted petrol prices during the test period

These visualizations provide a visual assessment of how closely the model follows observed petrol price movements.

---

## 🧪 Scenario Analysis

A scenario model was developed using the same key lagged predictors:

* Brent lag 1
* Brent lag 2
* USD/PKR lag 1

The scenario analysis can be used to explore how different assumptions about external economic conditions may affect predicted petrol price changes.

This provides a practical application of the regression model beyond historical analysis.

---

## 📷 Key Visualizations

The `outputs/` folder contains the major visualizations generated throughout the project:

* Correlation heatmap
* Petrol price vs. Brent crude oil
* Petrol price vs. USD/PKR
* Brent lag analysis
* USD/PKR lag analysis
* Monthly change correlation
* Lagged change correlations
* Actual vs. predicted changes
* Forecast test-period results
* Actual vs. predicted petrol prices
* Scenario analysis

---

## 📁 Project Structure

```text
Pakistan-Petrol-Price-Analytics/
│
├── notebooks/
│   └── Pakistan_Petrol_Price_Analytics.ipynb
│
├── outputs/
│   ├── actual_vs_predicted_changes.png
│   ├── actual_vs_predicted_prices.png
│   ├── brent_lag_analysis.png
│   ├── correlation_heatmap.png
│   ├── forecast_test_period.png
│   ├── lagged_change_correlations.png
│   ├── monthly_change_correlation.png
│   ├── petrol_vs_brent.png
│   ├── petrol_vs_usdpkr.png
│   ├── scenario_analysis.png
│   └── usdpkr_lag_analysis.png
│
├── README.md
│
└── requirements.txt
```

---

## ▶️ How to Run the Project

### 1. Clone the repository

Clone or download this GitHub repository to your computer.

### 2. Install the required libraries

Open a terminal in the project directory and run:

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

Open:

```text
notebooks/Pakistan_Petrol_Price_Analytics.ipynb
```

using Jupyter Notebook, JupyterLab, or another compatible environment.

### 4. Run the analysis

Run the notebook cells sequentially to reproduce the data analysis, regression models, forecasts, and visualizations.

---

## 💡 Key Takeaways

This project demonstrates a complete data analytics workflow applied to a real-world economic problem.

The analysis shows that:

* Brent crude oil prices have a significant relationship with petrol price changes.
* Lagged Brent crude oil variables provide additional explanatory information.
* The USD/PKR exchange rate is also statistically significant in explaining petrol price changes.
* Adding lagged variables improved the explanatory power of the regression model.
* The final forecasting model achieved an **R² of 0.370** on the training data.
* Scenario analysis can be used to examine potential petrol price movements under different economic conditions.

---

## 👨‍💻 Author

**Muhammad Hamza Ali**

Data Analytics | Python | SQL | Data Visualization

---

⭐ **Explore the notebook and visualizations to see the complete analysis and forecasting workflow.**
