🏡 Housing Price Prediction
📌 Project Overview

This project predicts California housing prices using machine learning techniques.
The dataset contains information such as the number of rooms, bedrooms, population, households, and the location’s proximity to the ocean.

We apply feature engineering, data preprocessing, and then train two models:

Linear Regression

Random Forest Regressor (with GridSearchCV optimization)

The goal is to compare their performance and evaluate which model predicts housing prices more accurately.

📂 Dataset

Dataset: housing.csv

Features include:

longitude, latitude

total_rooms, total_bedrooms

population, households

median_income

ocean_proximity (categorical)

Target variable:

median_house_value

⚙️ Steps in the Project
1. Data Preprocessing

Handle missing values (total_bedrooms → filled with median).

Train-test split (80% train, 20% test).

One-hot encoding for categorical variable (ocean_proximity).

Log transformation for skewed numerical features.

Feature scaling using StandardScaler.

2. Feature Engineering

Created new meaningful features:

bedroom_ratio = total_bedrooms / total_rooms

household_rooms = total_rooms / households

3. Model Training

Linear Regression: trained on standardized features.

Random Forest: trained with hyperparameter tuning (GridSearchCV).

4. Evaluation

Metric: R² score on test data.

Compared performance of Linear Regression and Random Forest.

📊 Results

Linear Regression: R² ≈ [your score here]

Random Forest (Best Model): R² ≈ [your score here]

👉 Random Forest performed better due to its ability to capture nonlinear relationships and feature interactions.
