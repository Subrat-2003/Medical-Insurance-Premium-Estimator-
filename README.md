# Medical Insurance Cost Prediction
### 📋 Project Overview
This project focuses on predicting individual medical insurance premiums using patient demographic and health data. By benchmarking **8 different Machine Learning algorithms**, the project identifies the most accurate regression model to estimate healthcare costs, offering a data-driven approach to premium calculation.

### 🎯 Objective
To engineer a robust regression pipeline that processes patient data and predicts insurance costs with high accuracy, optimizing over a baseline Linear Regression model.

### 📊 Dataset
* **Records:** 1,338 patients
* **Features:** Age, Sex, BMI, Children, Smoker, Region, Charges

### 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, XGBoost
* **Techniques:** Regression Analysis, Feature Engineering, Outlier Detection

### ⚙️ Methodology

1.  **Data Preprocessing:**
    * Handled missing values and verified data integrity.
    * **Outlier Treatment:** Applied **Interquartile Range (IQR) capping** to neutralize extreme values in `BMI` and `Charges`, ensuring model stability.
    * **Feature Engineering:** Implemented **One-Hot Encoding** for categorical variables (`Region`, `Sex`, `Smoker`) to convert qualitative data into machine-readable format.

2.  **Model Benchmarking:**
    * Evaluated 8 algorithms: Linear Regression, Decision Tree, Random Forest, SVR, KNN, AdaBoost, Gradient Boosting, and XGBoost.
    * Used **$R^2$ Score** as the primary evaluation metric.

### 📈 Model Performance
The analysis revealed that ensemble methods significantly outperformed linear models due to non-linear relationships in the data (e.g., the compounding cost impact of smoking).

| Model | $R^2$ Score | Performance |
| :--- | :--- | :--- |
| **Gradient Boosting Regressor** | **87.8%** | **🏆 Best Model** |
| Random Forest Regressor | ~85.0% | Strong Contender |
| XGBoost Regressor | ~81.0% | Good |
| **Linear Regression (Baseline)** | **77.1%** | Baseline |

### 💡 Key Insights
* **Gradient Boosting** achieved the highest accuracy (**87.8%**), providing a **~10% performance uplift** over the baseline Linear Regression model.
* **Smoking status** was identified as the strongest predictor of high insurance charges, introducing non-linearity that simple linear models struggled to capture effectively.
* **IQR Capping** was crucial for reducing the Mean Squared Error (MSE) by preventing outlier premiums from skewing the prediction line.

### 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/yourusername/medical-premium-estimator.git](https://github.com/yourusername/medical-premium-estimator.git)
    ```
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run the notebook:
    ```bash
    jupyter notebook Insurance_Analysis.ipynb
    ```
