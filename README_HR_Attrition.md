# 🧑‍💼 HR Employee Attrition Prediction

A machine learning project that predicts whether an employee is likely to leave a company, using the IBM HR Analytics dataset. The goal is to help HR teams identify at-risk employees early and take proactive retention measures.

---

## 📌 Problem Statement

Employee attrition is costly for organisations. This project builds and compares multiple classification models to predict attrition and identify the key factors driving it.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas | Data manipulation & cleaning |
| NumPy | Numerical operations |
| Seaborn & Matplotlib | Data visualisation |
| Scikit-Learn | Model building & evaluation |

---

## 📂 Dataset

- **Source:** IBM HR Analytics Employee Attrition & Performance dataset
- **Records:** 1,470 employees
- **Target variable:** `Attrition` (Yes / No → encoded as 1 / 0)
- **Features include:** Age, Department, Job Role, Monthly Income, Years at Company, Work-Life Balance, and more

---

## 🔍 Workflow

1. **Exploratory Data Analysis (EDA)**
   - Attrition distribution visualisation
   - Correlation heatmap of numeric features
   - Statistical summary of all variables

2. **Feature Engineering**
   - Converted target variable to binary (Yes → 1, No → 0)
   - Binned `YearsAtCompany` into career stage groups (0–2, 2–5, 5–10, 10+)
   - Dropped non-predictive columns (`EmployeeNumber`, `EmployeeCount`, `Over18`, `StandardHours`)
   - One-hot encoded all categorical variables

3. **Model Building & Comparison**

| Model | Accuracy | F1-Score | ROC-AUC |
|-------|----------|----------|---------|
| Logistic Regression | — | — | — |
| Random Forest | — | — | — |
| Gradient Boosting | — | — | — |

> Results populated after running the notebook.

4. **Feature Importance**
   - Identified top 10 drivers of attrition using Random Forest feature importances
   - Visualised as a horizontal bar chart

---

## 📊 Key Insights

- Models were compared across Accuracy, F1-Score, and ROC-AUC to account for class imbalance
- Feature importance analysis revealed the most influential factors in employee attrition
- Binning tenure into career stages improved model signal for early-career vs senior employees

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/hr-attrition-prediction.git
cd hr-attrition-prediction

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# 3. Add the dataset
# Place 'Employee-Attrition.csv' in the project folder

# 4. Open the notebook
jupyter notebook HR_Attrition_Analysis.ipynb
```

---

## 📁 Project Structure

```
hr-attrition-prediction/
│
├── HR_Attrition_Analysis.ipynb   # Main notebook
├── Employee-Attrition.csv        # Dataset (not included, download below)
└── README.md
```

📥 Dataset available at: [Kaggle — IBM HR Analytics](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

---

## 👤 Author

**Kgalalelo Kubheka**
Junior Data Scientist | Johannesburg, South Africa
📧 kgalalelokubheka@gmail.com
