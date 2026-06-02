# House Price Prediction using Supervised Learning

## Project Overview

This project focuses on predicting house prices using different supervised learning techniques. The objective is to analyze the relationship between property features and house prices and compare the performance of multiple regression models.

The project includes data preprocessing, exploratory data analysis, model implementation, evaluation, optimization using Gradient Descent techniques, and bias-variance analysis.

---

## Dataset Information

**Dataset Name:** RealEstate House Price Dataset

### Features

| Feature              | Description                          |
| -------------------- | ------------------------------------ |
| house_id             | Unique house identifier              |
| area_sqft            | House area in square feet            |
| bedrooms             | Number of bedrooms                   |
| bathrooms            | Number of bathrooms                  |
| location_score       | Location quality score               |
| age_years            | Property age in years                |
| distance_city_km     | Distance from city center            |
| lot_size_sqft        | Plot size in square feet             |
| has_garage           | Garage availability (0/1)            |
| has_pool             | Pool availability (0/1)              |
| renovation_years_ago | Years since last renovation          |
| house_price_inr      | House price in INR (Target Variable) |

### Target Variable

* **house_price_inr**

---

## Objectives

* Understand supervised learning concepts.
* Perform exploratory data analysis.
* Implement Simple Linear Regression.
* Implement Multiple Linear Regression.
* Implement Polynomial Regression.
* Evaluate model performance using regression metrics.
* Implement Gradient Descent optimization techniques.
* Analyze bias-variance trade-off.
* Identify the best-performing model.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Project Workflow

### Part A – Conceptual Understanding

Theoretical concepts covered:

* Supervised Learning
* Regression vs Classification
* Simple Linear Regression
* Linear Regression Assumptions
* Bias-Variance Trade-off
* Overfitting and Underfitting

---

### Part B – Dataset Understanding & Preparation

Tasks performed:

* Loaded and explored the dataset.
* Identified independent and dependent variables.
* Generated pairplot visualizations for exploratory analysis.
* Split the dataset into training and testing sets.

---

### Part C – Simple Linear Regression

Implemented Simple Linear Regression using:

* **Feature:** `area_sqft`
* **Target:** `house_price_inr`

Tasks completed:

* Model training
* Prediction generation
* Regression line visualization
* Residual analysis
* Interpretation of slope and intercept

---

### Part D – Model Evaluation

The Simple Linear Regression model was evaluated using:

* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score
* Adjusted R² Score

These metrics were used to measure prediction accuracy and model effectiveness.

---

### Part E – Multiple Linear Regression

Implemented Multiple Linear Regression using all available features.

Tasks completed:

* Model training
* Prediction generation
* Performance evaluation
* Comparison with Simple Linear Regression

### Observation

Multiple Linear Regression outperformed Simple Linear Regression because it utilized all relevant property features instead of relying only on house area.

---

### Part F – Polynomial Regression

Implemented Polynomial Regression using:

* Feature: `area_sqft`
* Degree: 2

Tasks completed:

* Polynomial feature transformation
* Model training
* Prediction generation
* Performance evaluation
* Comparison with Linear Regression

### Observation

Polynomial Regression produced results very similar to Simple Linear Regression and did not significantly improve prediction performance on this dataset.

---

### Part G – Gradient Descent Optimization

Implemented three optimization techniques:

#### Batch Gradient Descent

* Uses the entire dataset before updating parameters.
* Stable but computationally slower.

#### Stochastic Gradient Descent (SGD)

* Updates parameters after every training example.
* Faster but more noisy.

#### Mini-Batch Gradient Descent

* Uses small batches of data.
* Balances speed and stability.

### Observation

Mini-Batch Gradient Descent provided the most practical balance between convergence speed and stability.

---

### Part H – Bias-Variance Analysis

The train and test R² scores were analyzed for all models.

#### Simple Linear Regression

* Higher bias
* Lower variance
* Signs of underfitting

#### Multiple Linear Regression

* Balanced bias and variance
* Strong generalization performance

#### Polynomial Regression

* Slightly lower bias
* No significant improvement over Simple Linear Regression

### Best Model

Multiple Linear Regression achieved the best balance between accuracy and generalization.

---

### Part I – Final Analysis

#### Best Performing Model

**Multiple Linear Regression**

Reasons:

* Highest R² score
* Lowest prediction errors
* Utilized all relevant features
* Good balance between bias and variance

#### Impact of Gradient Descent

Gradient Descent improved model optimization by iteratively updating parameters to minimize prediction error.

#### Business Interpretation

The following factors were found to significantly influence house prices:

* House area
* Number of bedrooms
* Number of bathrooms
* Location score
* Property characteristics

These insights can assist real estate businesses in estimating property prices more accurately and supporting data-driven decision-making.

---

## Key Findings

* House area alone is insufficient for highly accurate predictions.
* Incorporating multiple property features significantly improves model performance.
* Multiple Linear Regression provided the most reliable results.
* Polynomial Regression did not offer meaningful improvement for this dataset.
* Mini-Batch Gradient Descent demonstrated an effective optimization strategy.

---

## Conclusion

This project successfully applied multiple supervised learning techniques for house price prediction. Among all models tested, Multiple Linear Regression delivered the best predictive performance due to its ability to utilize multiple property-related features simultaneously. The results demonstrate the importance of feature selection and model evaluation when building predictive machine learning solutions.

---

## Future Improvements

* Feature engineering and feature selection
* Cross-validation techniques
* Regularization methods (Ridge and Lasso)
* Ensemble learning models
* Advanced regression algorithms
* Hyperparameter optimization
