# predict-car-price
# Used Vehicle Valuation & Depreciation Analysis

## Research Question
Can a machine learning model accurately estimate the current market value of a used vehicle and forecast its depreciation over the next three years based on specific car features and projected annual mileage?

---

## Data Source(s)
The primary data will be sourced from the **Vehicle Dataset on Kaggle** (or data used in Capstone 2), which contains historical sales data including:
* **Year** (Age of the vehicle)
* **Selling Price** (Target variable)
* **Present Price** (Original MSRP)
* **Kilometers Driven** (Mileage)
* **Fuel Type & Transmission**

---

## Techniques for Analysis
I plan to use a multi-stage regression approach to handle both the current valuation and the future forecast:

1.  **Data Preprocessing:** Handling missing values and encoding categorical variables (e.g., brand, fuel type).
2.  **Exploratory Data Analysis (EDA):** Utilizing correlation matrices to identify which features most heavily impact price (e.g., age vs. mileage).
3.  **Regression Modeling:** Implementing **Random Forest Regressor** or **XGBoost** to capture the non-linear relationship between a car’s age and its price.
4.  **Time-Series Forecasting:** Developing a depreciation function that applies the trained model iteratively to predict price drops over a 3-year horizon based on user-defined usage patterns.



---

## Expected Results
The expected outcome is a functional model that provides a **"Fair Market Value"** for any input car. Additionally, the model will generate a **3-year "Value Outlook" report**, showing a predicted price curve that helps users understand how much equity they might lose (or keep) depending on how much they drive.

---

## Importance of the Question (Business Intelligence)
For most people, a car is one of the largest financial investments they will ever make, yet it is an asset that loses value every single day.

### What happens if this question is unanswered?
Without accurate forecasting, buyers and sellers are **"flying blind."** * A buyer might overpay for a car about to experience a steep drop in value.
* A seller might list a car too low and lose thousands in potential profit.
* Consumers may find themselves **"underwater"** on car loans—owing more than the car is worth—due to a lack of depreciation awareness.

### What benefit will this analysis bring?
This analysis transforms raw data into **Financial Clarity**.

* **For the Individual:** It acts as a financial planning tool. If you know a certain car will lose 40% of its value in three years but another only 15%, you can make a smarter purchase that protects your savings.

> **The Goal:** By distilling complex market trends into a simple 3-year forecast, we empower regular people to treat their vehicle purchase like a calculated investment rather than a stressful gamble.
