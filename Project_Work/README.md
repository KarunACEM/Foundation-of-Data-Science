# Loan Approval Prediction using Logistic Regression
A machine learning project that predicts whether a loan will be approved based on applicant details, financial information, and demographic factors. The project includes exploratory data analysis (EDA), data preprocessing, feature engineering, logistic regression model implementation from scratch, and comprehensive evaluation.

Team Name: FOD-Team
Member:Karun Rajbanshi (Roll No: ACE081BCT035)

## Problem Definition
The goal of this project is to predict loan approval status (Approved or Rejected) based on applicant information such as income, loan amount, credit history, and property area.

This is a binary classification problem, making logistic regression an appropriate model choice. The target variable is:
Loan_Status
Y = Loan Approved
N = Loan Rejected

## Dataset Description
Dataset Name: train.csv

## Features

### Feature	Description
- Gender:Male or Female
- Married:Marital status of applicant
- Dependents:Number of dependents
- Education:Graduate / Not Graduate
- Self_Employed:Employment status
- ApplicantIncome:Income of the applicant
- CoapplicantIncome:Income of co-applicant
- LoanAmount:Loan amount requested
- Loan_Amount_Term:Duration of the loan in months
- Credit_History:1 = Good, 0 = Bad
- Property_Area:Urban / Semiurban / Rural

### Target Variable:
Loan_Status (Y = Approved, N = Rejected)

### Dataset Source:
Loan Prediction Dataset on Kaggle(https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)

## Project Structure
Project Work/
├── README.md           # Project overview and instructions
├── eda.ipynb           # Exploratory Data Analysis and visualization
├── main.ipynb          # Data preprocessing, model training, and evaluation
└── loan_data.csv       # Raw dataset

## Installation

### Prerequisites
- Python 3.7 or higher
- Jupyter Notebook or VS Code with Jupyter extension

### Install Required Libraries
- pip install pandas numpy matplotlib seaborn scikit-learn jupyter

### Usage
- Open the project folder in VS Code or Jupyter Notebook
- Run eda.ipynb to perform exploratory data analysis and visualizations
- Run main.ipynb to preprocess data, train the logistic regression model, and evaluate results

## Methodology

1. Exploratory Data Analysis (EDA)

- Distribution plots for numerical features
- Countplots for categorical features
- Missing value analysis
- Correlation heatmap
- Outlier detection using boxplots

2. Data Preprocessing

- Fill missing values (median for numerical, mode for categorical)
- Feature engineering: Total Income, Income per Dependent, Loan-to-Income ratio
- One-hot encoding for categorical variables
- Scaling numerical features using StandardScaler
- Train-test split (80% train, 20% test)

3. Logistic Regression Implementation

- Sigmoid function
- Cross-entropy loss
- Gradient descent for weight updates
- Training loss visualization

4. Model Evaluation

- Accuracy, Precision, Recall, F1 Score
- ROC-AUC
- Confusion Matrix
- True vs Predicted visualization

## Results

The logistic regression model achieved the following performance on the test set:

Metric	Score
Accuracy	0.82
Precision	0.80
Recall	0.78
F1-Score	0.79
ROC-AUC	0.85

## Key Observations:

- Credit history strongly influences loan approval
- Applicants with higher income are more likely to get approved
- Property area also affects approval probability

## Features

- Exploratory Data Analysis with visualizations
- Data preprocessing and handling missing data
- Categorical variable encoding and feature scaling
- Logistic Regression model implemented from scratch
- Model evaluation using multiple metrics

## Future Improvements

- Hyperparameter tuning
- Using advanced models such as Random Forest or XGBoost
- Handling class imbalance
- Adding more features to improve accuracy
- Cross-validation for robust evaluation

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

## License
This project is for academic purposes.

## Acknowledgments
- Dataset used for educational purposes
- Built using Python libraries: pandas, numpy, matplotlib, seaborn, scikit-learn
- Inspired by loan prediction and financial analytics projects