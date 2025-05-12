# Grocery-Sales-Analysis & Predictive Modeling

## Project Overview

This project involves a comprehensive analysis of the "Supermart Grocery Sales - Retail Analytics Dataset". The primary objectives were to uncover sales trends, understand customer behavior, identify key performance drivers, and build foundational predictive models for net sales and customer segmentation. The analysis leverages Python and its data science ecosystem for data cleaning, exploratory data analysis (EDA), RFM segmentation, market basket analysis, time series forecasting, and machine learning.

## Dataset

*   **Description:** The dataset contains transactional data from a supermart, including information about orders, customers, products, categories, sales, discounts, and profits.
*   **File:** `Supermart Grocery Sales - Retail Analytics Dataset (1).csv`


## Key Analyses & Models Implemented

1.  **Data Cleaning & Preprocessing:**
    *   Handled inconsistent date formats and missing values.
    *   Engineered new features such as `Net Sales`, `COGS`, `Profit Margin (%)`, and various time-based features (Year, Month, DayOfWeek).
2.  **Exploratory Data Analysis (EDA):**
    *   Visualized overall sales, profit, and order volume trends (monthly and daily).
    *   Analyzed product performance by Category and Sub-Category.
    *   Assessed geographical performance by Region and City.
    *   Investigated the impact of discounts on profit margins and sales volume.
3.  **Customer Segmentation (RFM Analysis):**
    *   Calculated Recency, Frequency, and Monetary values for each customer.
    *   Developed RFM scores and segmented customers into categories like 'Champions', 'Loyal Customers', 'At Risk', etc.
    *   Visualized segment distribution and their monetary value.
4.  **Market Basket Analysis:**
    *   Utilized Apriori algorithm and association rules (Mlxtend) to identify frequently co-purchased items and potential cross-selling opportunities.
5.  **Sales Forecasting (Time Series):**
    *   Developed SARIMA and Prophet models to forecast daily net sales.
    *   Evaluated forecast accuracy using MAE, RMSE, and MAPE.
6.  **Predictive Modeling (Machine Learning):**
    *   **Net Sales Prediction:** Built a Random Forest Regressor (Scikit-learn) to predict transaction-level net sales.
        *   Features used: [List key features, e.g., Discount, Category, Region, Time features]
    *   **Customer RFM Segment Prediction:** Developed a Random Forest Classifier (Scikit-learn) to predict customer RFM segments.
        *   Features used: Recency, Frequency, MonetaryValue
        

## Technologies & Libraries Used

*   **Programming Language:** Python 3.x
*   **Core Libraries:**
    *   Pandas: Data manipulation and analysis.
    *   NumPy: Numerical computations.
    *   Matplotlib & Seaborn: Data visualization.
*   **Machine Learning & Statistics:**
    *   Scikit-learn: For RFM preprocessing, regression, classification, and metrics.
    *   Statsmodels: For SARIMA time series modeling.
    *   Prophet (by Facebook): For time series forecasting.
    *   Mlxtend: For Market Basket Analysis (Apriori).
*   **Other Tools:**
    *   Jupyter Notebook / Python script execution environment.
    *   Git & GitHub: Version control and repository hosting.


## How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/[YOUR_USERNAME]/[YOUR_REPOSITORY_NAME].git
    cd [YOUR_REPOSITORY_NAME]
    ```
2.  **Ensure Python and necessary libraries are installed.** You might want to use a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    pip install pandas numpy matplotlib seaborn statsmodels prophet mlxtend scikit-learn
    ```
3.  **Place the dataset** `Supermart Grocery Sales - Retail Analytics Dataset (1).csv` in the root directory of the project if it's not already there.
4.  **Run the Python script:**
    ```bash
    python grocery_sales_analysis.py
    ```
5.  Generated plots will be saved in the `plots/` directory.


## Future Work & Potential Improvements

*   Hyperparameter tuning for all predictive models (Regression, Classification, Time Series) to potentially improve performance.
*   Explore advanced feature engineering techniques for the Net Sales regression model.
*   Implement more sophisticated customer segmentation beyond RFM (e.g., K-Means clustering on behavioral data).
*   Develop a more interactive dashboard (e.g., using Streamlit or Dash) to present findings.
*   Investigate the root causes for variations in profit margins across different sub-categories and cities.

## Contact

*   **Name:** Abbas Ali Patel
*   **Email:** p.abbasali5@gmail.com
