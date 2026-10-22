# FUTURE_ML_01

## Machine Learning Internship – Task 1: Sales and Demand Forecasting

### Project Overview
This project uses machine learning to analyze historical retail sales and forecast future sales using Linear Regression.

### Objectives
- Clean and preprocess retail transaction data.
- Aggregate transaction-level data into monthly sales totals.
- Visualize historical sales trends.
- Train and evaluate a Linear Regression model.
- Forecast sales for future months.

### Dataset
The project uses a retail sales dataset downloaded from Kaggle. Transaction records include dates, product categories, quantities, prices, and total amounts.

The data was aggregated into monthly sales totals. January 2024 was excluded because it contained only two transactions and was likely incomplete.

### Tools and Technologies
- Python
- Google Colab
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- Linear Regression

### Methodology
1. Load and inspect the dataset.
2. Clean missing values and duplicate records.
3. Convert transaction dates into datetime format.
4. Aggregate sales by month.
5. Use the month sequence as a model feature.
6. Train on the first nine months and test on the last three months of 2023.
7. Evaluate predictions using MAE and RMSE.
8. Forecast sales for January to March 2024.

### Model Evaluation
- **Mean Absolute Error (MAE):** 10,870.28
- **Root Mean Squared Error (RMSE):** 11,986.63

These errors indicate that the baseline model has limitations and its forecasts should be interpreted cautiously.

### Limitations
The model uses only 12 complete monthly observations and a simple Linear Regression approach. It does not explicitly account for seasonal patterns or other factors affecting sales. More historical data and alternative models could improve forecasting performance.

### Project File
- `sales_forecasting.ipynb` — Notebook containing data preprocessing, visualization, model training, evaluation, and forecasting.

### Conclusion
This project demonstrates a basic machine learning workflow for retail sales forecasting and highlights how historical sales data can be used to estimate future demand.

