**Project Overview**

This project applies Machine Learning Regression techniques to predict car prices using the UCI Automobile Dataset — a classic dataset originally sourced from the UCI Machine Learning Repository.

The goal is to build predictive models that answer two practical, real-world questions:


**"Do I know if the dealer is offering fair value for my trade-in?"**
 **"Do I know if I put a fair value on my car?"**



By understanding the relationship between car features (such as engine size, horsepower, and fuel efficiency) and price, this model provides an objective estimate of what a car should cost.


**Objectives**


Load and explore the UCI Automobile dataset
Clean and prepare data for modelling
Perform Exploratory Data Analysis (EDA) to understand feature–price relationships
Build multiple regression models to predict car price
Evaluate and refine models for best performance



**Dataset**

Property Details Source UCI Machine Learning Repository Dataset UCI Automobile Dataset (imports-85.data)URLhttps://archive.ics.uci.edu/ml/machine-learning-databases/autos/imports-85.dataRows205Columns26Target Variableprice. 
Note: The dataset is loaded directly from the UCI repository URL — no local CSV file needed.

**Key Features Used:**

Feature Description make Car manufacturer (e.g. audi, toyota)engine-sizeSize of the enginehorsepowerEngine horsepowerhighway-mpgFuel efficiency on highwaycity-mpgFuel efficiency in citycurb-weightWeight of the car width Width of the car bodyfuel-typeGas or diesel drive-wheels fwd / rwd / 4wdbody-styleSedan, hatchback, convertible, etc.

**Methodology**

Step 1 — Data Loading & Inspection


Load the dataset directly from the UCI URL using pandas
Assign all 26 column names manually (dataset has no header row)
Inspect data types, missing values (? placeholders), and distributions


Step 2 — Data Wrangling


Replace ? with NaN and handle missing values
Convert columns to correct data types (e.g. price, horsepower to numeric)
Drop or impute rows with missing target values


Step 3 — Exploratory Data Analysis (EDA)


Correlation analysis to identify features most related to price
Regression plots and scatter plots to visualise feature–price relationships
Boxplots to explore categorical features (e.g. drive-wheels, body-style) vs price


Step 4 — Model Development

Models built progressively from simple to complex:

ModelDescriptionSimple Linear RegressionSingle feature (e.g. engine-size) vs priceMultiple Linear RegressionAll relevant numerical featuresPolynomial RegressionCaptures non-linear feature–price relationshipsRidge RegressionRegularised model to reduce overfitting

Step 5 — Model Evaluation & Refinement


Train/test split to assess generalisation
R² score and Mean Squared Error (MSE) as evaluation metrics
Cross-validation for robust performance assessment
GridSearchCV / parameter tuning for Ridge Regression



**Sample Results**

ModelR² Score (approx.) Simple Linear Regression (engine-size) ~ 0.76 Multiple Linear Regression ~ 0.82 Polynomial + Pipeline ~ 0.89Ridge Regression (tuned) ~ 0.88


Results are approximate and may vary based on train/test split and preprocessing choices.



**How to Run**

Prerequisites

bashpip install pandas numpy scikit-learn matplotlib seaborn jupyter

Steps


Clone the repository


bashgit clone https://github.com/lamide-akanni/PRICE-PREDICTION-USING-MACHINE-LEARNING-REGRESSION.git
cd PRICE-PREDICTION-USING-MACHINE-LEARNING-REGRESSION


Launch Jupyter Notebook


bashjupyter notebook


Open and run the main notebook — the dataset loads automatically from the UCI URL, no file download needed.



**Key Learnings**


Real-world datasets often contain missing values disguised as symbols (e.g. ?) that must be handled before modelling
engine-size, curb-weight, and horsepower are among the strongest predictors of car price
Polynomial features significantly improve model fit on non-linear relationships
Ridge regularisation helps prevent overfitting when using many features


**Connect:**
___________________________________________________________________________________________________________________________________________________________________
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/olamide-akanni-b240ab18a/)
[![Substack](https://img.shields.io/badge/Substack-FF6719?style=for-the-badge&logo=substack&logoColor=white)](https://substack.com/@lamideakanni03)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:akannilmd@gmail.com)




