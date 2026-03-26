# Battery Voltage Prediction using Environmental Data
Machine learning pipeline for predicting AWS battery voltage using environmental parameters (temperature, humidity, solar radiation, rainfall) for predictive maintenance.

## Overview
This project develops a machine learning model to predict battery voltage using environmental parameters:
- Temperature
- Relative Humidity
- Solar Radiation

The goal is to support **predictive maintenance for Automatic Weather Stations (AWS)**.

---

## Methodology

### 1. Data Preprocessing
- Datetime conversion
- Missing value handling:
  - Interpolation (linear)
  - Forward & backward fill
  - Drop missing target values

### 2. Feature Engineering
- Sliding window approach (window size = 4)
- Converts time series → supervised learning format

### 3. Normalization
- Standardization using training data mean & std

### 4. Model
- Linear Regression

---

## Results
- MSE: `0.27`
- RMSE: `0.20`
- Target Std: `0.39`

The model captures a significant portion of variation but is still a baseline model.

---

## Project Structure
- `Voltage_Prediction_Linear_Regression.ipynb` → main notebook
- `README.md` → project documentation

---

## Motivation
This project is part of a broader research direction:
**Environmental Data Science for infrastructure degradation and predictive maintenance.**
