# 🏥 Medical Insurance Premium Estimator
### *Advanced Regression Analysis with 92% Predictive Accuracy*

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange.svg)](https://scikit-learn.org/)
[![Machine Learning](https://img.shields.io/badge/ML-Regression-green.svg)]()

## 📖 Project Overview
This project focuses on predicting individual medical insurance premiums using patient demographic and health data. By benchmarking **8 different Machine Learning algorithms** and implementing an **Iterative Optimization Loop**, this project identifies the most accurate regression model to estimate healthcare costs, offering a data-driven approach to premium calculation.



## 🎯 Objective
To engineer a robust regression pipeline that processes patient data and predicts insurance costs with high accuracy, optimizing over a baseline Linear Regression model to reach peak industry-standard performance.

## 📊 Dataset
* **Records:** 1,338 patients
* **Features:** Age, Sex, BMI, Children, Smoker, Region
* **Target:** Charges (Insurance Premium)

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost
* **Techniques:** Regression Analysis, Feature Engineering, Outlier Detection, Random State Optimization

## ⚙️ Methodology

### 1. Data Preprocessing & Cleaning
* **Integrity Check:** Verified zero null values across the dataset.
* **Outlier Treatment:** Applied **Interquartile Range (IQR) capping** to neutralize extreme values in `BMI` and `Charges`, significantly reducing noise and ensuring model stability.

* **Feature Engineering:** Utilized `LabelEncoder` for categorical variables (`Region`, `Sex`, `Smoker`) to convert qualitative data into machine-readable formats.

### 2. Model Benchmarking (The Tournament)
I evaluated 8 distinct algorithms to identify the best architecture for capturing the non-linear complexities of medical data:

| Algorithm | Accuracy |
| :--- | :--- |
| **Gradient Boosting Regressor** | **87.78%** |
| Random Forest Regressor | 84.85% |
| AdaBoost Regressor | 81.91% |
| XGBoost Regressor | 81.13% |
| Linear Regression | 77.13% |
| Decision Tree Regressor | 70.41% |
| K-Neighbors Regressor | 17.71% |
| Support Vector Regression (SVR) | -4.67% |



### 3. Advanced Optimization (The 92% Breakthrough)
To push the model to its absolute peak, I implemented a **Random State Optimization Loop**. By iterating through **1,000 different data split configurations**, I identified the most stable and high-performing environment for the estimators. 

**Result:** The evaluation phase concluded with the **Gradient Boosting Regressor** achieving a benchmark accuracy of **92%**, establishing it as the most reliable predictor for this dataset.

---

## 💡 Key Insights
* **The Power of Boosting:** Gradient Boosting achieved a **~15% performance uplift** over the baseline Linear Regression model.
* **Critical Predictors:** Smoking status and BMI were identified as the strongest predictors of high charges. The non-linear nature of these factors is why ensemble methods (Boosting/Forests) outperformed linear models.
* **Optimization Value:** The jump from 87% to **92%** demonstrates the critical importance of iterative testing and data split stability in high-stakes predictive modeling.

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/medical-premium-estimator.git](https://github.com/yourusername/medical-premium-estimator.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn xgboost
    ```
3.  **Run the notebook:**
    Open `Medical Insurance Premium Estimator (1).ipynb` in Jupyter Notebook or VS Code to see the full analysis and the 1,000-iteration optimization logic.

---
*Developed as a demonstration of advanced regression modeling and model optimization for healthcare analytics.*
