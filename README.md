# Data_Analyst_intern
HR Attrition Analysis __Predicition and Visualizations of HR data using Python and PowerBI
# HR Attrition Analysis: Python + Power BI

This project performs a full-scale HR attrition analysis using **Python** for data exploration, machine learning, and SHAP interpretability, and integrates the results into **Power BI** for interactive visualization.

---

## 📌 Overview

- 🔍 Predict why employees leave the company (attrition)
- 🧪 Perform EDA and build a classification model in **Python**
- 🧠 Interpret model predictions with **SHAP (Explainable AI)**
- 📊 Visualize outcomes interactively in **Power BI**

---

## 📁 Dataset

**File**: `WA_Fn-UseC_-HR-Employee-Attrition.csv`  
**Source**: IBM HR Analytics Employee Attrition & Performance Dataset  
**Target Variable**: `Attrition` (`Yes`/`No` → encoded as `1`/`0`)

---

## ⚙️ Tools & Technologies

| Technology | Purpose |

|------------|---------|

| Python     |  Data analysis, modeling, SHAP explainability |

| Pandas, Seaborn, Matplotlib | Data wrangling & visualization |

| Scikit-learn | Machine learning (Random Forest) |

| SHAP       | Model interpretability |

| Power BI   | Dashboard & report generation |

---

## 🔧 Python Workflow

1. **Data Preprocessing**
   - Dropped irrelevant features (`EmployeeNumber`, `Over18`, etc.)
   - Converted categorical variables using `pd.get_dummies`
   - Encoded target column `Attrition`

2. **Exploratory Data Analysis (EDA)**
   - Distributions, correlations, and boxplots grouped in subplots
   - Feature importance plot from Random Forest

3. **Modeling**
   - Used `RandomForestClassifier` to predict attrition
   - Evaluated with confusion matrix and classification report

4. **Model Interpretability**
   - Used `SHAP` to explain global and local feature contributions
   - SHAP summary and dependence plots provided insights

5. **Power BI Export**
   - Added predicted attrition probability to each employee
   - Exported to CSV for Power BI integration

---

## 📊 Power BI Dashboard

The exported file `attrition_dashboard_data.csv` is used in Power BI to:
- Visualize attrition distribution
- Slice attrition risk by department, gender, and job role
- Show key features driving attrition risk using SHAP outputs
- Enable dynamic filtering by age, income, and overtime

---

## 📂 Files in Repository

├── HR_Attrition_Analysis.ipynb # Jupyter Notebook: EDA + ML + SHAP
├── HR-Employee-Attrition.csv # Raw dataset
├── attrition_dashboard_data.csv # Exported file with attrition probabilities
├── PowerBI_Dashboard.pbix # Power BI Dashboard file
└── README.md # Project overview

## 📦 Installation

Install Python dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn shap
🚀 Usage
In Python
Run HR_Attrition_Analysis.ipynb step by step.

Visualizations and SHAP plots will be rendered in the notebook.

A CSV file attrition_dashboard_data.csv will be created.

In Power BI
Open Power BI Desktop.

Load attrition_dashboard_data.csv.

Build visualizations using columns like:

Attrition_Prob

Age, Department, OverTime, etc.

📷 Sample Visualizations
🔥 Feature importance via Random Forest

📌 SHAP summary and dependence plots

🎯 Attrition risk segmented by business unit

📈 Attrition probability histogram in Power BI

👨‍💻 Author
## Rahul Babu Koppula

Connect for collaborations or questions.

### Want Help?

Would you like help:
- Creating a `.gitignore` and `requirements.txt`?
- Uploading the notebook and CSV to a GitHub repo?
- Designing visuals in Power BI based on your exported file?

Let me know how you'd like to proceed!
