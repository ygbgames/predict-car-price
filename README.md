# Project Proposal: Predictive Car Valuation & Depreciation Forecasting

## Research Question
Can a machine learning model accurately estimate the current market value of a used vehicle and forecast its depreciation over the next three years based on specific car features and projected annual mileage?

---

## Data Source(s)
The primary data is sourced from the **Vehicle Dataset (Kaggle)**, which provides a robust foundation of historical sales data. 
* **Key Features:** Year of manufacture, current selling price, original showroom price, kilometers driven, fuel type, transmission type, and seller type.
* **Target Variable:** `Selling_Price` (Current Market Value).

---

## Importance of the Question (Business Intelligence)
For most consumers, a vehicle is one of their largest financial investments, yet it is a rapidly depreciating asset. 

* **The Risk of No Analysis:** Without accurate forecasting, buyers and sellers are "flying blind." Buyers risk overpaying for vehicles facing steep depreciation curves, while sellers may lose thousands in potential profit. Crucially, this leads to consumers becoming "underwater" on loans—owing more than the car's actual worth.
* **The Strategic Benefit:** This analysis transforms raw market data into **Financial Clarity**. 
    * **For Individuals:** It serves as a financial planning tool, allowing users to choose vehicles that protect their savings (e.g., choosing a car with 15% depreciation over one with 40%).
    * **For the Market:** It replaces a "stressful gamble" with a calculated investment strategy.

---

## Techniques for Analysis
The project employs a multi-stage data science pipeline to bridge the gap between current value and future outlook:

1.  **Data Preprocessing:** Cleaning missing values, removing outliers in the `Present_Price` vs `Selling_Price` ratio, and encoding categorical variables like Brand and Fuel Type.
2.  **Exploratory Data Analysis (EDA):** Utilizing correlation matrices and scatter plots to quantify the impact of age vs. mileage. 
3.  **Regression Modeling:** Implementing **Random Forest Regressor** and **XGBoost** to capture non-linear relationships in automotive depreciation.
4.  **Time-Series Forecasting:** Developing a custom depreciation function that applies the trained model iteratively to predict price drops over a 3-year horizon based on user-defined annual mileage.

---

## Initial EDA Findings (from `car_valuation_eda.ipynb`)
Based on the initial analysis of the dataset:
* **Feature Correlation:** There is a high positive correlation between `Present_Price` and `Selling_Price`, as expected. 
* **Negative Impact of Age:** The data confirms a sharp decline in value within the first 5 years of ownership, after which the curve begins to flatten.
* **Transmission Influence:** Automatic variants consistently command a higher resale premium compared to manual counterparts in the current dataset.



---

## Expected Results
The final outcome will be a functional model that provides:
1.  **Fair Market Value:** A real-time appraisal based on the current state of the vehicle.
2.  **3-Year Value Outlook:** A generated report showing a predicted price curve, helping users visualize their equity position over a 36-month window.

---

## Repository Structure
* `car_valuation_eda.ipynb`: Contains the primary data exploration, cleaning, and visualization.
* `data/`: (If available) Contains the raw and processed CSV files.
