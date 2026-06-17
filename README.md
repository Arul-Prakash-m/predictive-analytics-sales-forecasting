# Predictive Analytics Using Historical Sales Data

## Project Overview

This project focuses on building predictive analytics models to forecast revenue trends using historical sales data. The workflow includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and comparison of machine learning algorithms.

The objective is to leverage historical sales patterns to generate accurate revenue predictions and identify the most effective predictive model.

---

## Business Objective

Organizations rely on historical sales data to make informed decisions regarding inventory planning, resource allocation, and revenue forecasting.

This project aims to:

- Analyze historical sales performance
- Identify seasonal revenue trends
- Build predictive models for revenue forecasting
- Compare machine learning algorithms
- Evaluate model performance using standard metrics

---

## Dataset Information

The dataset contains historical sales records with the following attributes:

| Column | Description |
|----------|-------------|
| Date | Transaction date |
| Product_Category | Product category |
| Region | Sales region |
| Units_Sold | Number of units sold |
| Unit_Price | Price per unit |
| Revenue | Total revenue generated |

### Engineered Features

Additional features were created from the Date column:

- Year
- Month
- Quarter
- DayOfWeek

---

## Data Preprocessing

The following preprocessing steps were performed:

- Loaded and inspected the dataset
- Checked for missing values
- Converted Date column to datetime format
- Created new time-based features
- Selected relevant features for modeling
- Split data into training and testing sets

---

## Exploratory Data Analysis (EDA)

### Monthly Revenue Trend

The monthly revenue analysis revealed clear seasonal patterns, with significant revenue peaks observed during November and December.

### Revenue by Product Category

Electronics generated the highest revenue among all product categories, making it the primary contributor to overall sales.

### Revenue by Region

Revenue distribution across regions was relatively balanced, with slight variations between regions.

---

## Machine Learning Models

### 1. Linear Regression

A Linear Regression model was initially trained using selected temporal and sales-related features.

After feature improvement by incorporating Unit_Price, model performance increased significantly.

### 2. Random Forest Regressor

A Random Forest Regressor was implemented to capture non-linear relationships within the data and improve forecasting accuracy.

---

## Model Performance Comparison

| Model | MAE | RMSE | R² Score |
|---------|---------:|---------:|---------:|
| Linear Regression | 58,018 | 87,642 | 0.916 |
| Random Forest Regressor | 1,085 | 3,301 | 0.99988 |

### Best Performing Model

**Random Forest Regressor** achieved the highest prediction accuracy with:

- R² Score: 0.99988
- Lowest MAE
- Lowest RMSE

This model was selected as the final forecasting model.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Project Structure

```text
predictive-analytics-sales-forecasting/
│
├── data/
│   └── sales_data.csv
│
├── notebooks/
│   └── predictive_analytics_sales_forecasting.ipynb
│
├── visuals/
│   ├── monthly_revenue_trend.png
│   ├── revenue_by_category.png
│   ├── revenue_by_region.png
│   └── actual_vs_predicted.png
│
├── requirements.txt
└── README.md
```

---

## Key Insights

- Revenue exhibits seasonal trends throughout the year.
- Electronics is the highest revenue-generating category.
- Feature engineering significantly improved model performance.
- Random Forest outperformed Linear Regression in forecasting accuracy.
- Historical sales data can effectively support data-driven forecasting decisions.

---

## Conclusion

This project demonstrates the complete predictive analytics workflow, from data preprocessing and exploratory analysis to machine learning model development and evaluation.

The Random Forest Regressor achieved exceptional forecasting performance with an R² Score of 0.99988, making it highly effective for revenue prediction based on historical sales data.

The project highlights the importance of feature selection, model comparison, and data-driven decision-making in predictive analytics.

---

## Author

**Arul Prakash M**

GitHub: https://github.com/Arul-Prakash-m
