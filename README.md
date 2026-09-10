# Pakistan Petrol Price Analytics & Forecasting

## 📌 Project Overview

This project analyzes and forecasts petrol price movements in Pakistan using historical petrol prices along with external economic factors such as **Brent crude oil prices** and the **USD/PKR exchange rate**.

The analysis explores relationships between these variables, examines lagged effects, develops predictive models, evaluates forecasting performance, and performs scenario analysis to understand potential changes in petrol prices.

## 🎯 Objectives

* Analyze historical petrol price trends in Pakistan.
* Examine the relationship between petrol prices and Brent crude oil prices.
* Analyze the relationship between petrol prices and the USD/PKR exchange rate.
* Investigate whether changes in external variables affect petrol prices with a time lag.
* Build a model to predict petrol price changes.
* Evaluate actual versus predicted results.
* Perform scenario analysis under different economic conditions.

## 🛠️ Technologies & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Statsmodels
* yfinance
* Requests
* OpenPyXL
* Jupyter Notebook

## 📊 Analysis Performed

### 1. Exploratory Data Analysis

The project begins by examining the dataset, including:

* Dataset structure and dimensions
* Variable information
* Missing values
* Descriptive statistics
* Historical petrol price movements

### 2. Correlation Analysis

Correlation analysis was performed to investigate relationships between:

* Petrol prices
* Brent crude oil prices
* USD/PKR exchange rate
* Other relevant numerical variables

A correlation heatmap was also created to visually summarize these relationships.

### 3. Brent Crude Oil Analysis

The project investigates the relationship between international crude oil prices and petrol prices in Pakistan.

The analysis includes:

* Petrol price vs. Brent crude oil
* Correlation analysis
* Lagged Brent crude oil relationships

### 4. USD/PKR Exchange Rate Analysis

The effect of exchange-rate movements on petrol prices was also examined through:

* Petrol price vs. USD/PKR analysis
* Correlation analysis
* Lagged USD/PKR relationships

### 5. Monthly Change Analysis

Monthly percentage changes were calculated to analyze how changes in petrol prices relate to changes in external economic variables.

The project includes:

* Monthly percentage-change correlations
* Lagged monthly change correlations
* Correlation visualizations

### 6. Predictive Modeling

A predictive model was developed to estimate petrol price changes using relevant explanatory variables.

Model performance was evaluated by comparing:

* Actual changes
* Predicted changes
* Actual prices
* Predicted prices

### 7. Forecast Evaluation

The model was evaluated over a test period to assess how closely the predictions followed the actual petrol price movements.

Visualizations compare actual and predicted values during the test period.

### 8. Scenario Analysis

Scenario analysis was performed to examine how different assumptions about external economic variables could affect petrol prices.

This provides a practical way to understand potential petrol price movements under different market conditions.

## 📈 Key Visualizations

The `outputs/` folder contains the major visualizations produced during the analysis:

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

## ▶️ How to Run

1. Clone or download this repository.
2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```text
notebooks/Pakistan_Petrol_Price_Analytics.ipynb
```

4. Run the notebook cells sequentially to reproduce the analysis and visualizations.

## 💡 Project Insights

This project demonstrates how Python-based data analytics can be used to study the relationship between domestic petrol prices and important international and macroeconomic factors.

The combination of correlation analysis, lag analysis, predictive modeling, forecast evaluation, and scenario analysis provides a broader understanding of petrol price dynamics in Pakistan.

## 👨‍💻 Author

**Muhammad Hamza Ali**

Data Analytics | Python | SQL | Data Visualization

---

⭐ If you find this project useful, feel free to explore the notebook and visualizations.
