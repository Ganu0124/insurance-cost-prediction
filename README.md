# 🏥 Predict Insurance Charges using ML

## Overview

Insurance companies determine premium amounts by evaluating various customer attributes such as age, gender, body mass index (BMI), smoking habits, number of dependents, and geographic region. Accurately estimating insurance charges is important for risk assessment and pricing strategies.

This project develops a Machine Learning-based predictive model that estimates medical insurance charges using historical customer data. Multiple regression algorithms are implemented and compared to identify the model that delivers the best prediction performance.

The project demonstrates the complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning, performance evaluation, and prediction generation.

---

## Problem Statement

Medical insurance costs vary significantly among individuals due to differences in health conditions, lifestyle choices, and demographic characteristics. Manual estimation of insurance premiums is time-consuming and may lead to inconsistent pricing decisions.

The objective of this project is to develop a predictive analytics solution that automatically estimates insurance charges based on customer information.

---

## Objectives

* Analyze insurance customer data.
* Perform exploratory data analysis.
* Understand relationships between features and insurance charges.
* Build multiple regression models.
* Compare model performance using evaluation metrics.
* Optimize model parameters using GridSearchCV.
* Generate accurate insurance cost predictions.
* Identify the most influential features affecting insurance premiums.

---

## Dataset Description

The dataset contains information about insurance beneficiaries and their corresponding medical insurance charges.

### Input Features

| Feature  | Description                               |
| -------- | ----------------------------------------- |
| Age      | Age of the customer                       |
| Sex      | Gender of the customer                    |
| BMI      | Body Mass Index                           |
| Children | Number of dependents covered by insurance |
| Smoker   | Smoking status                            |
| Region   | Residential region                        |

### Target Variable

| Variable | Description               |
| -------- | ------------------------- |
| Charges  | Medical insurance charges |

### Dataset Statistics

* Total Records: 1338
* Total Features: 6 Input Features + 1 Target Variable
* Data Type: Structured Tabular Data
* Learning Type: Supervised Learning
* Problem Type: Regression

---

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to understand data distribution, identify patterns, and discover relationships among variables.

The following visualizations were generated:

### Insurance Charges Distribution

Shows the distribution of medical insurance charges across all customers.

### Age vs Charges

Analyzes the relationship between age and insurance costs.

### BMI vs Charges

Examines the impact of body mass index on insurance premiums.

### Smoker vs Charges

Compares insurance charges between smokers and non-smokers.

### Correlation Heatmap

Visualizes relationships between numerical features and the target variable.

---

## Data Preprocessing

Several preprocessing techniques were applied before model training:

### Missing Value Analysis

The dataset was inspected for missing values to ensure data quality.

### Categorical Encoding

Categorical variables such as:

* Sex
* Smoker
* Region

were converted into numerical values using Label Encoding.

### Feature Selection

Relevant features were selected for model training while the target variable was separated.

### Train-Test Split

The dataset was divided into:

* 80% Training Data
* 20% Testing Data

This ensures proper model evaluation on unseen data.

---

## Machine Learning Models Implemented

### Linear Regression

Linear Regression serves as a baseline model for predicting insurance charges.

Advantages:

* Simple implementation
* Fast training
* Easy interpretation

### Decision Tree Regressor

Decision Trees learn hierarchical relationships between features and insurance costs.

Advantages:

* Captures nonlinear relationships
* Easy visualization
* Handles feature interactions

### Random Forest Regressor

Random Forest combines multiple decision trees to improve prediction accuracy and reduce overfitting.

Advantages:

* High prediction accuracy
* Robust performance
* Better generalization

---

## Hyperparameter Tuning

GridSearchCV was applied to optimize the Random Forest model.

Parameters such as:

* Number of Trees (n_estimators)
* Maximum Tree Depth (max_depth)

were tuned to identify the best-performing model configuration.

This process improved overall model performance and prediction accuracy.

---

## Model Evaluation

The models were evaluated using the following metrics:

### R² Score

Measures how well the model explains variation in insurance charges.

### Mean Absolute Error (MAE)

Measures average prediction error.

### Root Mean Squared Error (RMSE)

Measures prediction accuracy while penalizing larger errors.

### Cross Validation

5-Fold Cross Validation was used to evaluate model stability and generalization performance.

---

## Feature Importance Analysis

Feature Importance analysis was performed using the Random Forest model.

This analysis helps identify which variables contribute most to insurance cost prediction.

Typical influential features include:

* Smoking Status
* Age
* BMI
* Number of Children
* Region
* Gender

---

## Prediction Analysis

Additional visualizations were generated to evaluate prediction quality.

### Actual vs Predicted Plot

Compares actual insurance charges with predicted values.

### Residual Distribution Plot

Analyzes prediction errors and model behavior.

### Sample Prediction

The trained model predicts insurance charges for new customer records.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Joblib
* Jupyter Notebook

---

## Repository Structure

insurance-cost-prediction-ml/

├── insurance_prediction.ipynb

├── insurance.csv

├── README.md

├── Project_Report.pdf

├── requirements.txt

├── LICENSE

└── .gitignore

---

## Key Learning Outcomes

* Data Cleaning and Preprocessing
* Exploratory Data Analysis
* Data Visualization
* Regression Modeling
* Hyperparameter Tuning
* Cross Validation
* Feature Importance Analysis
* Model Evaluation
* Predictive Analytics

---

## Conclusion

This project successfully demonstrates the application of machine learning techniques for predicting medical insurance charges. Multiple regression models were trained and compared, with the Tuned Random Forest Regressor providing the best predictive performance. The project highlights the importance of feature engineering, model optimization, and evaluation techniques in building accurate predictive analytics solutions .

---

## Author

Ganesh M

