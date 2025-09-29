# End-to-End Customer Churn Prediction

This repository contains the code and analysis for an end-to-end machine learning project focused on predicting customer churn for a telecommunications company. This project demonstrates a complete data science workflow, from data cleaning and exploratory data analysis to model building and evaluation.

---

## 🚀 Project Goal
The primary objective is to build a reliable classification model that can identify customers who are likely to churn. This allows the business to develop targeted retention strategies to reduce revenue loss and improve customer loyalty.

---

## 📊 Dataset
The analysis is based on the Telco Customer Churn dataset, which contains customer account information, demographic data, and subscribed services.

---

## 🛠️ Methodology & Workflow
1.  **Data Cleaning:** Handled missing values (in `TotalCharges`) and corrected data types.
2.  **Exploratory Data Analysis (EDA):** Visualized data to uncover key predictors of churn, such as:
    * Customers with **Month-to-Month Contracts**.
    * Customers with **Fiber Optic** internet service.
    * Customers **without** key add-on services like `OnlineSecurity` and `TechSupport`.
3.  **Preprocessing & Feature Engineering:**
    * Converted categorical features into a numerical format using one-hot encoding.
    * Scaled numerical features (`tenure`, `MonthlyCharges`) using `StandardScaler`.
4.  **Modeling & Evaluation:**
    * A baseline **Decision Tree** model was first established.
    * A more robust **Random Forest** model was trained, which showed improved accuracy.
    * The class imbalance in the dataset was addressed using **SMOTE** (Synthetic Minority Over-sampling Technique).
    * The final Random Forest model was re-trained on the balanced data.

---

## 📈 Results
The final SMOTE-balanced Random Forest model proved to be the most effective, achieving:
* **AUC Score:** 0.81
* **Churn Recall:** 61%

This represents a significant improvement in identifying at-risk customers compared to the baseline models, fulfilling the project's primary objective.

---

## 📂 Repository Contents
* `End Customer Churn Prediction.ipynb`: The main Jupyter Notebook with all the code and analysis.
* `README.md`: This project summary file.

