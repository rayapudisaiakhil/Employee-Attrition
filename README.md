# Employee Attrition Prediction

This project aims to predict employee attrition using machine learning classifiers on HR dataset.

## Problem Statement

- HR datasets contain useful insights into factors affecting employee satisfaction and retention. 

- Being able to predict employee attrition can help organizations take proactive retention measures.

- Supervised classifiers are trained on the dataset to predict the probability of attrition.

## Data

- The dataset contains 14999 rows and 10 features like department, monthly hours, projects, evaluation, satisfaction etc.

- It has a class imbalance with 87% samples being 'Employed' and 13% being 'Left'

- Missing value imputation and outlier removal are done during data cleaning.  

## Exploratory Data Analysis

- Satisfaction, last evaluation and tenure have maximum variability among features.

- Employees with tenure > 6 years are removed as outliers not indicative of general behavior.

- Null values are imputed using mean/mode or new categories like 'other' department. 

## Feature Engineering

- Categorical variables like department and salary are encoded into dummy variables.

- Numerical variables are standardized using StandardScaler.

- Train-test split is done with stratification to handle class imbalance.

## Modeling

The following models are trained and evaluated:

- Decision Tree Classifier
- Random Forest Classifier
- KNearest Neighbors
- Logistic Regression
- Gradient Boosting Classifier

Hyperparameter tuning is done using RandomizedSearchCV and GridSearchCV.

## Results

- Random Forest yields best performance with 98% accuracy and 97% recall. 

- Decision tree and GBM also perform well with over 90% accuracy.

- Most important factors are satisfaction, evaluation, monthly hours, department and salary.

## Conclusion

The project demonstrates effectively applying machine learning for employee churn prediction. The workflow can be replicated for other HR analytics tasks.

## Usage

The analysis is in Python. To replicate:

- Clone the repository
- Install dependencies from requirements.txt
- Run the Jupyter notebook
