# Medical Insurance Cost Prediction

This project performs a comprehensive analysis of health insurance data to predict the medical charges for individuals based on various demographic and health-related features. 

## 📊 Project Overview
The goal of this analysis is to identify the key factors that influence insurance premiums and build a predictive model to estimate costs accurately. The notebook includes data cleaning, exploratory data analysis (EDA), and machine learning model implementation.

## 📂 Dataset Information
The dataset consists of **1,338 records** with the following features:
- **Age**: Age of the primary beneficiary.
- **Sex**: Insurance contractor gender (female, male).
- **BMI**: Body Mass Index, providing an understanding of body weight relative to height.
- **Children**: Number of children covered by health insurance / Number of dependents.
- **Smoker**: Smoking status (yes, no).
- **Region**: The beneficiary's residential area in the US.
- **Charges (Target)**: Individual medical costs billed by health insurance.

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost.

## 📈 Key Findings & Results
- **Data Integrity**: The dataset contained no missing values (NaNs), ensuring a clean start for the analysis.
- **Modeling**: Several regression models were tested, including XGBoost.
- **Performance**: The best-performing model achieved an accuracy score of approximately **0.81** (R-squared), indicating strong predictive power.

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
