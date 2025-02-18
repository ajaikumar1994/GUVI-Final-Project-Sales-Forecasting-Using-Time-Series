# GUVI Final Project: Time Series Sales Forecasting

This project forecasts department-wide sales for each store for the upcoming year, modeling the impact of markdowns on holiday weeks. The analysis provides actionable recommendations for inventory management, resource allocation, and strategic decision-making.

## Project Overview

Accurate sales forecasting is crucial for retail success. This project leverages time series analysis, specifically the Prophet model by Facebook, to predict future sales trends.  The model incorporates both long-term trends and seasonal patterns, including the effects of markdowns during holiday periods, to generate more accurate and insightful forecasts.

## Goals

1. **Sales Forecasting:** Predict department-wide sales for each store for the following year.
2. **Markdown & Holiday Impact:** Model the effects of markdowns on sales during holiday weeks.
3. **Actionable Recommendations:** Provide data-driven recommendations for optimizing inventory, resource allocation, and strategic planning.

## Methodology

1. **Data Preprocessing:**
    * Data cleaning and feature engineering (combining markdown columns, creating holiday dataframe).
    * Train/test split.
2. **Model Training:**
    * Training the Prophet model on historical sales data.
    * Incorporating holiday effects and multiplicative seasonality.
3. **Forecasting:**
    * Generating future sales forecasts.
    * Aggregating forecasts to weekly levels.
4. **Analysis & Visualization:**
    * Evaluating model performance using RMSE and relative RMSE.
    * Visualizing forecasts, trend, and seasonality using Plotly and Matplotlib.
    * Analyzing the impact of holidays on sales and markdowns.
5. **Recommendation Generation:**
    * Developing prioritized recommendations based on forecast insights.

## Code Structure

* `sales_forecast`: Contains the `sales_forecast` function for generating sales predictions.
* `holiday_effect.py`: Contains the `holiday_effect` and `Markdown_holiday_effect` functions for analyzing holiday impacts.
* `sales_forecasting_prophet.ipynb`: Jupyter Notebook containing the main analysis, model training, visualization, and recommendation generation.


## How to Run

1. Clone the repository: `git clone https://github.com/ajaikumar1994/GUVI-Final-Project-Sales-Forecasting-Using-Time-Series.git`
2. Install required libraries:
3. Run the Jupyter Notebook: `sales_forecasting_prophet.ipynb`

## Key Findings & Recommendations 

* **Upward Sales Trend:** Sales are generally increasing over time.
* **Seasonal Patterns:**  Sales peaks are observed in January, March, September, November, and December.

**Prioritized Recommendations:**

1. **Leverage Seasonal Demand (High Priority):**
    * Target marketing campaigns around high-sales months.
    * Increase promotions and discounts before peak demand periods.
2. **Optimize Inventory Management (High Priority):**
    * Stock up before high-sales months.
    * Reduce excess inventory before sales dips.
3. **Pricing & Markdown Strategy (Medium Priority):**
    * Increase markdowns before slow months.
    * Optimize markdowns during peak months.
4. **Holiday-Specific Promotions (Medium Priority):**
    * Special promotions during November and December.
    * Targeted discounts or exclusive product launches in January and March.
5. **Improve Forecasting & Supply Chain Planning (Low Priority):**
    * Ensure suppliers are prepared for increased seasonal demand.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

 MIT License
