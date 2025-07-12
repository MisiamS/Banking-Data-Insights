# Banking-Data-Insights

## Overview
This project performs Exploratory Data Analysis (EDA) and data cleaning on a dataset from a direct marketing campaign conducted by a banking institution. The dataset is structured to support potential classification models that predict whether a customer will subscribe to a bank term deposit based on various features.

## Objectives
- Assess and enhance the quality of the dataset.
- Explore patterns and key feature relationships.
- Prepare clean and reliable data for future ML modeling.

## Techniques Used
- Data Quality Assessment
- Missing Value Handling
- Encoding
- Feature Exploration & Group-wise Aggregations
- Visualization with Matplotlib & Seaborn
- Skewness and Outliers Handling


## Dataset
- Source: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
- Features include customer demographics, contact strategies, campaign outcomes, and macroeconomic context.
- Target Variable: `subscribed` (whether a customer subscribed to a term deposit: `yes` / `no`)

##  Data Preparation Highlights
- **Missing Value Treatment:** Identified and handled missing or special-case entries in features such as `age`, `pdays`, `poutcome`, `job`, `education`, and `contact`.
- **Categorical Encoding:** Applied label encoding and one-hot encoding to transform nominal categorical variables (e.g., `job`, `marital`, `housing`, `loan`, `default`) into numerical formats suitable for modeling.
- **Cyclical Encoding:** Used sine and cosine transformations for cyclical features
- **Outlier Detection & Handling:** Visualized and addressed outliers in continuous variables such as `age` and `balance` using filtering and domain reasoning.
- **Skewness Correction:** Applied transformations (e.g., log scaling) to reduce skewness in heavily skewed numeric variables, improving distributional balance.
- **Feature Interpretation:** Handled special cases such as `pdays = -1` to represent clients not previously contacted, ensuring these were logically consistent with related fields like `poutcome`.
- **Data Cleaning:** Removed invalid entries, standardized categorical values, and ensured a clean, analysis-ready dataset.

## Results
- Identified and addressed data quality issues, improving dataset integrity.
- Explored variable distributions and customer behavior patterns.
- Prepared a clean dataset suitable for training ML models to predict subscription likelihood.
