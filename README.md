# 🌫️ PM2.5 Pollution Level Classification Using Weather Data

This repository contains the code, dataset reference, and results of the project **"PM2.5 Pollution Level Classification Using Machine Learning with Random Forest and Gradient Boosting"**. The goal is to classify air quality levels based on PM2.5 concentrations using weather data as input features.

## 📌 Project Overview

PM2.5 (particulate matter ≤ 2.5μm) is one of the most harmful pollutants affecting public health. This project focuses on **classifying PM2.5 pollution levels** using machine learning, helping to build early warning systems and environmental awareness.

## 📊 Dataset

- **Source**: [Kaggle - Air Quality & Weather Dataset](https://www.kaggle.com/)  
  
- **Features Include**:
  - PM2.5 concentration (target, later classified into categories)
  - Temperature
  - Humidity
  - Wind Speed
  - Dew Point
  - Atmospheric Pressure
  - and other meteorological indicators

- **Label Mapping**:
  PM2.5 values are converted into AQI categories based on international standards:
  | Category       | PM2.5 Range (µg/m³) |
  |----------------|---------------------|
  | Good           | 0 – 50              |
  | Moderate       | 51 – 100            |
  | Unhealthy      | 101 – 150           |
  | Very Unhealthy | 151 – 200           |
  | Hazardous      | > 200               |

## ⚙️ Methods Used

1. **Data Preprocessing**
   - Handling missing values
   - Normalization and label encoding
   - Mapping PM2.5 values into categorical AQI levels

2. **Classification Algorithms**
   - 🌲 **Random Forest**
   - 🌟 **Gradient Boosting Regressor (GBR)** (used for classification by mapping predicted values to categories)

3. **Evaluation Metrics**
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix

4. **Validation**
   - Train-test split (80/20 or 70/30)
   - Optionally using K-Fold Cross Validation
