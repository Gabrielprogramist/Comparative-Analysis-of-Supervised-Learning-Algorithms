## Overview
This project performs a comparative analysis of multiple supervised learning algorithms for predicting insurance expenses. The analysis is based on the `insurance.csv` dataset provided as part of the **"Mathematics for Data Science" course (Assignment 5)**. The goal is to predict the insurance expenses using features such as **age**, **sex**, **BMI**, **number of children**, and **smoking status**.

---

## Project Structure

├── insurance.csv # The dataset file.
├── Comparative_Analysis_of_Supervised_Learning_Algorithms_on_Insurance_Expenses.ipynb # The Jupyter Notebook containing the code.
├── Report.pdf # The final report with analysis, results, and discussion.
└── README.md # This README file.

---

## Requirements
- **Python 3.x**
- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn

### Installation
You can install the required libraries using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn

**How to Run**

1.  Place the `insurance.csv` file in the same directory as the Jupyter Notebook.
2.  Run the `Comparative_Analysis_of_Supervised_Learning_Algorithms_on_Insurance_Expenses.ipynb` file.

**Description**

**Data Preprocessing:**

*   Column names are standardized to lowercase.
*   Categorical features (`sex` and `smoker`) are converted to the 'category' data type.
*   Numerical features (`age`, `bmi`, and `children`) are scaled using `StandardScaler`.
*   Categorical features are encoded using `OneHotEncoder` (with `drop='first'`).
*   The dataset is split into 80% training and 20% testing sets.

**Model Training and Evaluation:**

The following regression models are implemented using scikit-learn’s `Pipeline`:

*   Linear Regression
*   Decision Tree Regressor
*   Random Forest Regressor
*   Support Vector Regressor (SVR)
*   Gradient Boosting Regressor

Model performance is evaluated using RMSE, MAE, and R². Hyperparameter tuning for Random Forest is performed using `GridSearchCV`.

**Visualization:**

A correlation heatmap is generated to understand the relationships among numerical features.

**License**

This project is intended for educational purposes. You are free to modify and redistribute the code.