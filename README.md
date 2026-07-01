# Employee Attrition Prediction 📊

A machine learning project that predicts whether an employee is likely 
to leave the company, using the IBM HR Analytics dataset. Built as part 
of a Data Science internship to help HR teams identify at-risk employees 
and take proactive retention decisions.

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (Logistic Regression, Random Forest, Gradient Boosting)
- Google Colab (Jupyter Notebook)

## 📁 Project Structure
EmployeeAttrition/
├── analysis.ipynb                        ← full notebook (EDA + ML)
├── WA_Fn-UseC_-HR-Employee-Attrition.csv ← IBM HR dataset (1470 employees)
├── charts/
│   ├── chart1_attrition_dept_role.png    ← attrition by department & role
│   ├── chart2_income_vs_attrition.png    ← income vs attrition
│   ├── chart3_confusion_matrix.png       ← model evaluation
│   ├── chart4_feature_importance.png     ← top 10 attrition factors
│   └── chart5_roc_curve.png             ← ROC curve (all 3 models)
└── summary.pdf                           ← project summary report

## 📊 Dataset
- **Source:** IBM HR Analytics Employee Attrition Dataset
- **Size:** 1,470 employees | 35 features
- **Target:** Attrition (Yes/No) — 16% attrition rate (imbalanced dataset)

## 🔍 What This Project Does

### 1. Data Preprocessing
- Removed irrelevant columns (EmployeeNumber, Over18, etc.)
- Handled class imbalance using class_weight='balanced'
- One-hot encoded categorical variables
- Scaled numeric features using StandardScaler

### 2. Exploratory Data Analysis (EDA)
- Attrition rate by Department and Job Role
- Monthly Income comparison between employees who stayed vs left
- Identified key patterns driving employee exits

### 3. Models Trained
| Model | Precision | Recall | F1 Score | ROC-AUC |
|---|---|---|---|---|
| Logistic Regression | ✅ Best | ✅ Best | ✅ Best | ✅ Best |
| Random Forest | - | - | - | - |
| Gradient Boosting | - | - | - | - |

**Best Model: Logistic Regression**

## 💡 Key Findings
- **1 in 6 employees** is likely to leave the company
- **Sales Representatives** have the highest exit rate (~40%)
- **Lower salary** is a strong predictor of attrition
- **Overtime work** is one of the top warning signs of resignation
- Most exits happen within the **first 2–3 years** of joining

## ✅ HR Recommendations
1. Launch a **New Employee Retention Program** for employees in their first 3 years
2. Introduce an **Overtime Monitoring Policy** to flag burnout risk early
3. Conduct **urgent salary reviews** for Sales and HR departments

## ⚠️ Limitation
This model predicts based on historical patterns — it cannot account for 
sudden life events or personal reasons. It should support HR decisions, 
not replace human judgment.

## 👩‍💻 Developed By
Sujithra S — BCA Student, Stella Maris College, Chennai  
Internship Project — Xylofy AI
