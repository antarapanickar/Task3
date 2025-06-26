# Task 3 - Housing Price Prediction (Linear Regression)

This is the third task in my AI and ML internship. The goal was to create a linear regression model to predict housing prices using a dataset from Kaggle. I worked with both simple and multiple linear regression and assessed the model's performance using standard metrics.

## About the Dataset

The dataset contains information about house features such as:

- Area
- Bedrooms, Bathrooms
- Stories, Parking
- Main Road Access, Guest Room, Basement, etc.
- Heating, AC, and Furnishing Status

Target column: price  
Dataset used: [Housing Price Prediction – Kaggle](https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction)

## What I Did

- Imported the dataset and checked for missing values (none found)
- Converted categorical columns using one-hot encoding
- Trained a Linear Regression model using Scikit-learn
- Evaluated the model using:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - R² Score
- Printed model coefficients to interpret feature impact
- Plotted actual vs predicted prices to visualize performance


## Model Evaluation

| Metric | Value |
|--------|-------|
| **MAE** | 970043.40 |
| **MSE** | 17,543,186,873.30 |
| **R² Score** | 0.6529 |


## Key Coefficients (Impact on Price)

| Feature | Coefficient |
|---------|-------------|
| Area | 2.359e+03 |
| Bedrooms | 7.677e+04 |
| Bathrooms | 1.094e+06 |
| Basement | 5.12e+05 |
| Air Conditioning | 2.67e+05 |
| Hot Water Heating | 4.99e+05 |
| Furnishing Status (Unfurnished) | -4.13e+05 |

*Note: Coefficients show how much each feature increases or decreases the price.*

## Visualization

I used a scatter plot to show how well the model predicted prices compared to actual prices based on area:

- **Green** = Actual Price  
- **Blue** = Predicted Price

It helped show that while the model picks up trends, it's not perfect (R² around 65%).


## Tools Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
