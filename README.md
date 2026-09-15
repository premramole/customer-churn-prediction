# 📊 Customer Churn Analysis & Prediction

**By Prem Ramole** | Data Analyst Portfolio Project

## 🎯 Project Objective
Analyzed customer churn patterns for a telecom company using exploratory data analysis, then built machine learning models to predict which customers are likely to churn.

**Dataset:** [Telco Customer Churn — Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

**Tools Used:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## 📌 Workflow
1. Data Loading & Overview
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Model Building (Logistic Regression + Random Forest)
6. Model Evaluation
7. Key Insights & Business Recommendations

## 📈 Key Findings
- **Overall churn rate: ~26.5%** — roughly 1 in 4 customers leave.
- **Month-to-month contract customers churn the most** — longer contracts reduce churn significantly.
- **Higher monthly charges correlate with higher churn.**
- **New customers (low tenure) are the most at-risk group.**
- **Top churn predictors:** Tenure, MonthlyCharges, TotalCharges, Contract type, InternetService.

## 🏆 Model Performance

| Model | Accuracy | ROC-AUC |
|---|---|---|
| Logistic Regression | 79.91% | 0.8403 |
| Random Forest | 79.21% | 0.8225 |

Logistic Regression slightly outperforms Random Forest here, likely because churn drivers in this dataset are fairly linear — a case where a simpler, interpretable model holds its own against a more complex one.

## ✅ Business Recommendations
- Offer loyalty discounts to month-to-month customers after 3 months.
- Target high-monthly-charge customers with retention offers.
- Focus onboarding efforts on the first 6 months (highest churn window).
- Use the model to flag at-risk customers proactively.

## 📁 Repository Contents
- `Customer_Churn_Project_Guide.ipynb` — full analysis notebook
- `churn_distribution.png`, `churn_by_contract.png`, `monthly_charges_churn.png`, `tenure_churn.png`, `correlation_heatmap.png`, `confusion_matrices.png`, `feature_importance.png` — visualizations generated during EDA and model evaluation
