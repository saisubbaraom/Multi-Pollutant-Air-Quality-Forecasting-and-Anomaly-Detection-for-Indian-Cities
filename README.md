# Air Quality Forecasting and Anomaly Detection using Time Series Analysis

## Project Overview

This project develops an end-to-end Air Quality Index (AQI) forecasting and anomaly detection framework using historical air quality monitoring data collected from Hyderabad monitoring stations.

The objective is to analyze historical pollution patterns, forecast future AQI levels, and identify unusual pollution events that deviate from expected behavior.

---

## Dataset Summary

* Total Records: 8,077
* Monitoring Stations: 5
* Time Period: 2016–2026
* Selected Station: Zoo Park, Hyderabad
* Target Variable: AQI

Pollutants included:

* PM2.5
* PM10
* NO₂
* SO₂
* CO
* O₃

---

## Project Workflow

### Data Quality Assessment

* Missing value analysis
* Station-level quality assessment
* Monitoring station selection

### Exploratory Data Analysis

* AQI distribution analysis
* AQI category analysis
* Dominant pollutant analysis
* Seasonal trend analysis

### Feature Engineering

* Lag features
* Rolling statistics
* Calendar features
* Cyclical month encoding

### Forecasting Models

* Naive Forecast
* Linear Regression
* Random Forest
* XGBoost

### Anomaly Detection

* STL Decomposition
* Residual Analysis
* Z-Score Based Anomaly Detection

---

## Key Findings

### Air Quality Characteristics

* Moderate AQI was the most common category.
* AQI ranged from 7.43 to 500.

### Dominant Pollutants

The most influential pollutants were:

1. PM10
2. PM2.5

### Seasonal Patterns

* Highest AQI observed during January–March.
* Lowest AQI observed during June–September.
* March recorded the highest average AQI.
* August recorded the lowest average AQI.

### Forecasting Results

| Model             | RMSE  |
| ----------------- | ----- |
| Linear Regression | 23.51 |
| Naive Forecast    | 24.85 |
| Random Forest     | 28.31 |
| XGBoost           | 31.38 |

Linear Regression achieved the best overall forecasting performance.

### Anomaly Detection

STL decomposition combined with statistical thresholding successfully identified unusual AQI events that could not be explained by normal trend or seasonal behavior.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Statsmodels
* Scikit-Learn
* XGBoost

---

## Future Enhancements

* Weather data integration
* Multi-step forecasting
* Multi-station forecasting
* Deep learning models (LSTM, GRU)
* Real-time dashboard deployment

---

## Author

Sai Subba Rao Mahendrakar
