# Churn Prediction Analysis and Model Development

This project involves a comprehensive analysis of customer churn data and the development of a predictive model to identify customers who are at risk of churning. The project utilizes various data analysis techniques, statistical tests, and machine learning models.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
   - Customer Demographics
   - Churn Analysis
   - Product Usage
   - Financial Analysis
4. [Predictive Modeling](#predictive-modeling)
   - Feature Engineering
   - Model Development
   - Hyperparameter Tuning
   - Model Evaluation
5. [Requirements](#requirements)
6. [How to Run](#how-to-run)
7. [Results](#results)
8. [Contributing](#contributing)
9. [License](#license)

## Project Overview

The goal of this project is to understand the factors influencing customer churn and develop a predictive model that can help identify customers who are at risk of leaving. The project includes:

- Data exploration and visualization.
- Statistical analysis to determine relationships between variables.
- Development and tuning of a machine learning model using XGBoost.
- Saving the trained model for future predictions.

## Dataset

The dataset used in this project contains customer information such as age, gender, geographical location, balance, credit score, and whether the customer has churned or not.

## Exploratory Data Analysis (EDA)

### Customer Demographics

1. **Age Distribution**: The distribution of customers across different age groups was visualized using a histogram.



2. **Gender Distribution**: The gender distribution of customers was analyzed using a pie chart.


### Churn Analysis

1. **Churn Percentage**: The percentage of customers who have churned was calculated.

2. **Reasons for Churn**: A chi-square test was performed to determine if there is a significant relationship between categorical variables (e.g., Geography, Gender, NumOfProducts) and customer churn.

3. **Churn Patterns**: Churn patterns were identified by analyzing the distribution of churned customers across different segments (e.g., Geography, Gender, Age).

### Financial Analysis

1. **Average Account Balance**: The average balance of customers was calculated.

2. **Financial Characteristics**: The financial characteristics of churned vs. non-churned customers were compared using histograms.

## Predictive Modeling

### Feature Engineering

- **Geography and Gender Encoding**: The `Geography` column was converted to boolean values using one-hot encoding, and the `Gender` column was mapped to binary values.

### Model Development

- **Initial XGBoost Model**: An XGBoost model was trained to compute feature importances, identifying the top 5 most significant predictors of customer churn.

### Hyperparameter Tuning

- **Grid Search**: Hyperparameter tuning was performed using GridSearchCV to find the best model configuration.

### Model Evaluation

- **Classification Report**: The final model was evaluated using a classification report, providing metrics such as precision, recall, and F1-score.

## Requirements

To run this project, you need the following Python libraries:

```bash
pandas
matplotlib
scipy
xgboost
scikit-learn
joblib
```

## How to Run

1. **Clone the Repository**: Clone this repository to your local machine.
2. **Install Dependencies**: Install the required Python libraries.
3. **Run the Script**: Execute the Jupyter notebook or Python script to perform the analysis and train the model.
4. **View Results**: The trained model will be saved as `model.pkl`, and you can use it for future predictions.

## Results

- The top 5 most significant predictors of customer churn were identified.
- A tuned XGBoost model was developed, achieving high accuracy in predicting at-risk customers.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.
