# Electricity-Consumption-Estimation
Key Findings from the Analysis

Electricity consumption has shown an upward trend from 1973 to 2019, indicating increasing energy usage over time.
Seasonal patterns are evident, with fluctuations in electricity consumption corresponding to specific months and years.
Quantitative Insights:

The average electricity consumption in early years (e.g., 1973) was around 35-40 TW, whereas in later years (e.g., 2019), it reached 100-120 TW.
Seasonal decomposition revealed additive components like trend, seasonality, and residuals, helping isolate year-round consumption patterns and anomalies.
Stationarity Check:

An Augmented Dickey-Fuller (ADF) test indicated that the time series is non-stationary. Transformation techniques, such as logarithmic differencing, improved stationarity.
Forecasting Model:

The Exponential Smoothing model was used for forecasting future electricity consumption.
Model evaluation using Mean Absolute Percentage Error (MAPE) showed a low error rate (~3%), validating its accuracy for predicting consumption.
Seasonal Trends:

Summer months showed higher electricity consumption, likely due to increased cooling demands.
Winter months exhibited slightly reduced consumption, pointing to variations in energy needs.
Future Forecasting:

The model predicts continuous growth in electricity consumption, with expected values reaching up to ~131 TW in peak months by 2020.
Approach Explained:
Data Cleaning and Preprocessing:

The data was indexed by date, and missing values (if any) were managed.
Time-based features (year, month) were extracted to facilitate seasonal analysis.
Exploratory Data Analysis:

Visualization of raw data trends using line graphs.
Pivot tables to summarize year-wise and month-wise data for comparative insights.
Seasonal Decomposition:

The data was decomposed into trend, seasonal, and residual components using the seasonal_decompose function.
Stationarity Testing:

ADF tests confirmed the need for transformations to stabilize the variance and mean.
Log and differencing transformations were applied.
Forecasting:

Exponential Smoothing (ETS) models with additive and multiplicative components were applied for forecasting.
Parameter tuning for alpha (level), beta (trend), and gamma (seasonality) improved model performance.
Validation:

The dataset was split into training and testing sets.
Model predictions were compared against actual values, with MAPE used as the accuracy metric.
Seasonality and Trend Analysis:

Seasonal peaks and troughs were examined to understand high-demand periods.
Quantitative Outputs:
1973 Average Consumption: ~35 TW
2019 Peak Consumption: ~122 TW
Forecast for 2020 Peak Month: ~131 TW
Seasonality Influence: ~10% variation between peak and trough months.
MAPE for Model Validation: ~3%
Recommendations:
Energy Planning: Plan infrastructure and supply to meet predicted future demand, especially during peak months.
Seasonal Preparedness: Address seasonal spikes by optimizing energy storage and generation capabilities.
Continuous Monitoring: Update models regularly with new data to refine forecasts.
Policy Implications: Focus on sustainable energy sources to handle growing demand effectively.
