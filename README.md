# LightForce Task Report

## Overview

This project involves analyzing and predicting power consumption across multiple parameters and locations. It consists of two main tasks:

1. Predicting next-day and scenario-based power consumption.
2. Consolidating energy consumption data across multiple locations using Power BI.

---

## Task 1: Power Consumption Prediction

**Dataset:** `test data(1).xlsx`  
Contains power consumption data for three days for various parameters of XYZ.

### Objectives
- Predict the next day’s consumption for all parameters.
- Provide scenario predictions for the next two days under different conditions.

### Approach
1. **Data Preparation**
   - Clean the dataset and handle missing values.
   - Extract relevant features such as date, time, daily sums, and averages.

2. **Modeling**
   - Apply regression models like **Random Forest** or **XGBoost** for predictions.
   - Optionally apply **PCA** for dimensionality reduction.
   - Use **Isolation Forest** for anomaly detection if required.

3. **Scenario Analysis**
   - Define scenarios:
     - **Normal:** Continuation of current trends.
     - **High Load:** Simulated increased usage.
     - **Low Load:** Simulated decreased usage.
   - Predict power consumption for the next two days under each scenario.

4. **Output**
   - `next_day_prediction.xlsx` → Predicted next-day values for all parameters.
   - `scenario_predictions.xlsx` → Scenario-based predictions for two days.
   - Visualizations highlighting trends and anomalies.

---

## Task 2: Consolidated Reporting using Power BI

**Dataset:** `Energy Consumptions.xlsx`  
Contains energy consumption data for **459 locations**.

### Objectives
- Create a comprehensive Power BI report consolidating data across all locations.
- Enable interactive analysis and insights for management.

### Approach
1. **Data Loading**
   - Import the Excel sheet into Power BI.
   - Clean and transform the data (handle missing values, rename columns, set proper data types).

2. **Data Modeling**
   - Create relationships if multiple tables exist.
   - Define calculated measures such as total consumption, average consumption, and peak load.

3. **Visualizations**
   - Dashboards for:
     - Total energy consumption by location
     - Trends over time
     - High vs. low consumption locations
     - KPI cards for quick insights

4. **Consolidated Reporting**
   - Summarize all 459 locations in a single report.
   - Include scenario insights, trends, and recommendations.

---

## Tools & Libraries

- **Python** (Task 1)
  - `pandas`, `numpy` → Data processing
  - `scikit-learn` → Machine learning
- **Power BI** (Task 2)
  - Data transformation, modeling, dashboard creation

---

