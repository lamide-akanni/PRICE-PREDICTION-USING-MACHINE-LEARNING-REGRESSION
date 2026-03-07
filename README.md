Car Price Prediction Using Regression Models
Project Overview

This project develops predictive models to estimate automobile prices using machine learning techniques. The workflow follows a standard data science pipeline including data acquisition, preprocessing, exploratory data analysis (EDA), feature selection, model development, and performance evaluation.

The objective is to understand how different automobile attributes influence price and to build regression models capable of predicting vehicle prices based on these features.



Dataset Source

UCI Machine Learning Repository – Automobile Dataset

Dataset Link - https://archive.ics.uci.edu/ml/machine-learning-databases/autos/imports-85.data

The target variable for prediction is price.

Key libraries used: pandas numpy matplotlib seaborn & scikit-learn

Data Cleaning and Preprocessing

Several preprocessing steps were applied to prepare the data for modeling:

Handling Missing Values

Missing values in the dataset were identified and addressed using appropriate strategies such as:

Replacing missing numeric values with statistical estimates

Removing rows where critical values were unavailable

Data Type Conversion

Columns such as:

price

horsepower

normalized-losses

were converted from object types to numeric types to allow mathematical operations.

Feature Selection

Relevant numerical predictors were selected for regression modeling based on correlation and domain relevance.
Exploratory Data Analysis (EDA)

Exploratory analysis was conducted to understand relationships between features and the target variable.

Visualization techniques used:

Scatter plots

Regression plots

Distribution plots

Correlation analysis

Example relationships explored:

Engine size vs Price

Highway MPG vs Price

Horsepower vs Price

These analyses helped identify the most influential predictors.

Model Development

Multiple regression techniques were implemented to model the relationship between automobile features and price.

1. Simple Linear Regression

A simple linear regression model was built using highway-mpg as the predictor variable.

Model structure:

Price = β0 + β1(Highway MPG)

This model helps illustrate the basic relationship between fuel efficiency and vehicle price.

2. Multiple Linear Regression

A multiple regression model was built using multiple predictors.

Example predictors:

normalized-losses

highway-mpg

Model structure:

Price = β0 + β1(Normalized Losses) + β2(Highway MPG)

This approach improves predictive capability by incorporating multiple features.

3. Polynomial Regression

Polynomial regression was used to capture non-linear relationships between variables and price.

This technique allows the model to fit curved relationships in the data rather than strictly linear trends.


Model Evaluation

Models were evaluated using standard regression metrics.

R² (Coefficient of Determination)

Measures how much variance in the price is explained by the model.

Higher R² indicates better model fit.

Mean Squared Error (MSE)

Measures the average squared difference between predicted and actual prices.

Lower MSE indicates better predictive accuracy.

Visualization of Results

Several visualization techniques were used to interpret model performance:

Regression Plots

Show the linear relationship between predictors and the target variable.

Distribution Plots

Compare the distribution of predicted prices versus actual prices.

Scatter Plots

Used to observe relationships between key variables.

Key Insights

Key findings from the analysis include:

Engine size and horsepower are strong predictors of vehicle price.

Fuel efficiency (highway MPG) tends to show a negative relationship with price.

Models using multiple predictors perform better than single-variable models.

Polynomial regression can capture nonlinear patterns in the data.

Technologies Used

Python

Libraries:

pandas

numpy

matplotlib

seaborn

scikit-learn

Development environment: Jupyter Notebook

Repository Structure
project-folder
│
├── DEVELOPING A MODEL.ipynb
├── README.md
└── requirements.txt (optional)


Future Improvements

Possible extensions to the project:

Feature engineering

Cross-validation

Regularized regression (Ridge, Lasso)

Tree-based models

Hyperparameter optimization

Deployment as a predictive API



Technologies Used

Python

Libraries:

pandas

numpy

matplotlib

seaborn

scikit-learn

Development environment:

Jupyter Notebook

Repository Structure
project-folder
│
├── DEVELOPING A MODEL.ipynb
├── README.md
└── requirements.txt (optional)


Future Improvements

Possible extensions to the project:

Feature engineering

Cross-validation

Regularized regression (Ridge, Lasso)

Tree-based models

Hyperparameter optimization

Deployment as a predictive API



Authur
Olamide,

Data Science / Machine Learning Project
