# Task 8 – Energy Consumption Time Series Forecasting

## Objective
Forecast household energy consumption using time series models (ARIMA, Prophet, XGBoost) to analyze trends, seasonality, and make accurate predictions of future energy usage.

## Approach
- Loaded the `household_power_consumption.csv` dataset and combined `Date` and `Time` columns into a single `Datetime` index.
- Handled missing values by forward-filling to maintain continuity in the time series.
- Resampled the data to daily averages of `Global_active_power` for consistent analysis.
- Performed Exploratory Data Analysis (EDA):
  - Plotted energy usage trends over time.
  - Examined correlations and seasonal patterns.
- Built and compared three forecasting models:
  - **ARIMA** for baseline statistical forecasting.
  - **Prophet** for capturing trend and seasonality.
  - **XGBoost** with engineered time-based features (day, month, year, weekday).
- Evaluated models using MAE and RMSE metrics.
- Visualized forecasts vs. actual energy consumption.

## Results & Insights
- **ARIMA** performed as a simple baseline but was limited in capturing complex seasonality.
- **Prophet** effectively modeled daily/seasonal patterns and provided interpretable trend insights.
- **XGBoost** delivered strong predictive accuracy when combined with engineered features.
- The models demonstrate clear energy usage patterns that can be applied for demand forecasting and energy efficiency planning.
