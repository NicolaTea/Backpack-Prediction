# **Backpack Price Prediction 🏒🎒**<br/>
In this project, the goal is to predict the price of backpacks based on various features such as compartments, weight capacity, brand, material, size, and more. The dataset consists of multiple attributes, which we use to train and evaluate models.<br/>

## **📊 Dataset**<br/>
  train.csv: Contains features and target variable (Price).<br/>
  test.csv: Contains features for prediction (no target variable).<br/>
  Key Features:
  1. Compartments
  2. Weight Capacity (kg)
  3. Brand
  4. Material
  5. Size
  6. Style
  7. Laptop Compartment
  8. Waterproof

## 🧠 Approach
Two models were implemented:

Baseline Model:<br/>
Algorithm: Linear Regression<br/>
Goal: Predict backpack prices based on basic preprocessing and feature handling.<br/>

Optimized Model:<br/>
Algorithm: Random Forest Regressor<br/>

Enhancements:<br/>
Feature Engineering: Created new features such as Price_per_kg, Density, Premium_Brand, Feature_Score, and Brand_Price_Ratio to better capture relationships between attributes.

## 🚀 Results
Baseline Model:<br/>
R-squared: 0.001<br/>
Mean Absolute Error (MAE): 33.65<br/>
Mean Squared Error (MSE): 1514.83<br/>
Model Performance: Poor due to simple model and limited features.<br/>

Optimized Model:<br/>
R-squared: 0.9999<br/>
Mean Absolute Error (MAE): 0.10<br/>
Mean Squared Error (MSE): 0.02<br/>
Model Performance: Excellent, showing a substantial improvement with Random Forest.<br/>

Key Feature Engineering Improvements:<br/>
Price_per_kg: Price divided by weight capacity to normalize pricing.<br/>
Density: Weight capacity divided by the number of compartments, providing a measure of efficiency.<br/>
Premium_Brand: Identified premium brands and created a binary feature to capture their influence on price.<br/>
Feature_Score: Created a score based on the presence of desirable features (like waterproof, laptop compartment, style).<br/>
Brand_Price_Ratio: Calculated the average price for each brand relative to the price per kg, helping to capture brand influence.<br/>

## 📈 Visualizations
Included visualizations to evaluate model performance and residuals:
1. Actual vs Predicted Prices (Scatter plot)
2. Distribution of Residuals (Histogram)
3. Feature Importance (Bar plot)

This project is part of a competition on Kaggle.
