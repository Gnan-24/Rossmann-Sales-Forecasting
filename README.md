# Rossmann Sales Forecasting Project

## 1. Project Objective
The goal of this project was to develop a machine learning model to accurately forecast daily sales for the Rossmann drug store chain. This helps in optimizing inventory, staffing, and promotional strategies.

## 2. Data Source
The data was provided by Rossmann for a public Kaggle competition. It can be downloaded directly from the [Rossmann Store Sales competition page on Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales/data).

## 3. Methodology
The project followed a standard data science workflow:
* **Data Cleaning:** Handled missing values in `CompetitionDistance` and `Promo2`-related fields. Filtered data to only include days when stores were open.
* **Exploratory Data Analysis (EDA):** Analyzed the relationships between sales and key variables like promotions, holidays, store type, and day of the week.
* **Feature Engineering:** Created new time-based features from the 'Date' column (Year, Month, WeekOfYear) and calculated the age of competing stores and ongoing promotions.
* **Modeling:**
    * Established a baseline model using Random Forest.
    * Developed an advanced model using **XGBoost** with early stopping to find the optimal number of boosting rounds.

## 4. Final Results
The final XGBoost model achieved a **Validation RMSPE (Root Mean Square Percentage Error) of 0.1614**. This was a significant improvement of over 50% compared to the initial baseline model, demonstrating the effectiveness of the feature engineering and modeling approach.

## 5. How to Run
1.  Clone this repository.
2.  Install the required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`.
3.  Run the `Rossmann_Analysis.ipynb` Jupyter Notebook.
