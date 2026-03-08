# Loan Approval Prediction using Logistic Regression

A comprehensive machine learning project that predicts whether a loan will be approved based on applicant details, financial information, and other factors. This project includes exploratory data analysis (EDA), data preprocessing, feature engineering, model training using logistic regression from scratch, and detailed evaluation.


## Table of Contents

- Overview
- Dataset
- Project Structure
- Installation
- Usage
- Methodology
- Results
- Features
- Dependencies
- Future Improvements
- License


## Overview

This project aims to predict loan approval status (approved or not) based on features such as applicant income, coapplicant income, loan amount, credit history, and demographic details. The model is built using logistic regression implemented from scratch with gradient descent.

**Key highlights of this project:**

- Logistic regression implemented from scratch without sklearn’s LogisticRegression
- Comprehensive EDA with multiple visualizations
- Feature engineering and preprocessing
- Model evaluation with multiple metrics (Accuracy, Precision, Recall, F1, ROC-AUC)
- Handles missing values and categorical variables


## Dataset

The dataset contains information about loan applicants and whether their loan was approved.

### Features

- **Gender** – Male or Female
- **Married** – Marital status of the applicant
- **Dependents** – Number of dependents
- **Education** – Graduate or Not Graduate
- **Self_Employed** – Employment status
- **ApplicantIncome** – Income of the applicant
- **CoapplicantIncome** – Income of co-applicant
- **LoanAmount** – Loan amount requested
- **Loan_Amount_Term** – Duration of the loan
- **Credit_History** – Credit history of the applicant
- **Property_Area** – Urban, Semiurban, or Rural

### Target Variable

- **Loan_Status**
  - Y = Loan Approved
  - N = Loan Not Approved


## Project Structure

Project Work
│
├── README.md
├── eda.ipynb
├── loan_data.csv
└── main.ipynb

- **eda.ipynb** → Exploratory Data Analysis and visualization  
- **main.ipynb** → Data preprocessing, model training, and evaluation  


## Installation

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or VS Code with Jupyter extension

### Install Required Libraries

Run the following command:
pip install pandas numpy matplotlib seaborn scikit-learn jupyter


## Usage

1. Open the project folder in **VS Code or Jupyter Notebook**
2. Open the notebook **eda.ipynb**
3. Run all cells to perform data analysis and visualization
4. Open **main.ipynb**
5. Run all cells to preprocess data, train the model, and evaluate results


## Methodology

### 1.Exploratory Data Analysis (EDA)

- Distribution of numerical features
- Countplots of categorical features
- Missing value analysis
- Correlation heatmap
- Outlier detection via boxplots

### 2.Data Preprocessing

- Fill missing values (median for numerical, mode for categorical)
- Feature engineering: Total Income, Income per Dependent, Loan-to-Income ratio
- One-hot encoding for categorical features
- Scaling numerical features using StandardScaler
- Train-test split (80% train, 20% test)

### 3.Logistic Regression Implementation

- Sigmoid function
- Cross-entropy loss
- Gradient descent for weight updates
- Training loss visualization

### 4.Model Evaluation

- Accuracy, Precision, Recall, F1 Score
- ROC-AUC
- Confusion Matrix
- True vs Predicted visualization


## Results

After training the logistic regression model, the model achieves a reasonable accuracy in predicting loan approval.

Key observations:

- Credit history strongly influences loan approval
- Higher income applicants are more likely to get loans approved
- Property area also affects approval probability

The confusion matrix helps visualize the number of correct and incorrect predictions.


## Features

Implemented features in this project:

- Exploratory Data Analysis with visualizations
- Data preprocessing pipeline
- Handling missing data
- Categorical variable encoding
- Feature scaling
- Logistic Regression model training
- Model evaluation using multiple metrics


## Future Improvements

Possible improvements for the project include:

- Hyperparameter tuning
- Using advanced models such as Random Forest or XGBoost
- Handling class imbalance
- Adding more features to improve prediction accuracy
- Cross-validation for better model evaluation


## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter


## License

This project is created for educational purposes as part of the Foundation of Data Science Lab course.


## Acknowledgments

- Dataset used for educational purposes
- Built using Python data science libraries including pandas, numpy, matplotlib, seaborn, and scikit-learn
- Inspired by loan prediction and financial analytics projects