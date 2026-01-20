# predict-car-price
# Used Vehicle Valuation & Depreciation Analysis

## Research Question / Business Problem 
Can a machine learning model accurately estimate the current market value of a used vehicle and forecast its depreciation over the next three years based on specific car features and projected annual mileage?

# Car Valuation Prediction & EDA

This repository contains a comprehensive Exploratory Data Analysis (EDA) and predictive modeling project aimed at estimating the market value of used cars. By leveraging historical vehicle data, the project identifies key price drivers and builds a regression framework for valuation.

## 🚀 Project Overview

The goal of this project is to understand how different vehicle attributes—such as mileage, age, engine capacity, and brand—influence the resale price prediction for a customer. The workflow is documented in the `car_valuation_eda.ipynb` notebook and includes:

* **Data Preprocessing:** Cleaning missing entries, handling duplicates, and formatting.
* **EDA:** Statistical analysis and data visualization using Seaborn and Matplotlib.
* **Feature Engineering:** Converting raw data into meaningful inputs (e.g., calculating vehicle age).
* **Modeling:** Implementation of machine learning algorithms to predict car prices using baseline model as Logistics Regression

## 📊 Dataset Highlights

The analysis focuses on several critical features:
- **Vehicle Age:** The impact of depreciation over time.
- **Mileage:** The correlation between distance driven and market price.
- **Specifications:** Influence of fuel type (Petrol/Diesel), Transmission (Manual/Automatic), and Engine displacement.
- **Brand Identity:** Price variations across different manufacturers.

## 🛠️ Requirements

To run the notebook and reproduce the analysis, you will need the following Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
