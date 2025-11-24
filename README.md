# EDA- PROJECT OVERVIEW 

# 📊 Exploratory Data Analysis (EDA) — End-to-End Project

### 📌 Workshop Project — Hands-On EDA with Python

This repository contains an **End-to-End Exploratory Data Analysis (EDA) workflow** using Python.  
You will learn how to transform raw data into clean, structured, and insightful information for model building and business decisions.

---

## 🧭 Agenda

| # | Topic |
|---|------|
| 1 | What is EDA & Why do we need it? |
| 2 | What is Raw Data |
| 3 | Missing Value Treatment |
| 4 | What is Clean Data |
| 5 | Create Dataset for Predictive Modeling |
| 6 | Variable Identification |
| 7 | Univariate Analysis |
| 8 | Bivariate Analysis |
| 9 | Outlier Detection |
|10 | Variable Creation / Encoding |
|11 | Build ML-Ready Dataset |

---

## 🧩 What is EDA?

EDA (Exploratory Data Analysis) is a process used to:

✔ Understand data structure  
✔ Detect anomalies & missing values  
✔ Identify patterns, relationships & distributions  
✔ Prepare data for machine learning  

> “Garbage in → Garbage out” 💡  
Clean data leads to better model accuracy!

---

## 🗂 What is Raw Data?

Raw data = **Unprocessed data** directly collected from:

- Customers
- Sensors
- Web Logs
- HTML, CSV, XML, APIs
- Databases

🚫 Cannot be visualized directly if:
- Too many missing values
- Formatting errors
- Mixed types

---

## 🧽 Data Cleaning

Data Cleaning = Detecting & fixing:

| Issue | Fix |
|------|----|
| Missing values | Mean/Median/Mode |
| Incorrect types | Type Conversion |
| Outliers | Capping / Removal |
| Noise | Filter / Smooth |
| Inconsistency | Standardization |

👉 Data cleaning is mandatory **before** visualization & ML.

---

## 📝 Example Missing Value Imputation

python
import pandas as pd

df['Age'].fillna(df['Age'].median(), inplace=True)
df['Season'].fillna(df['Season'].mode()[0], inplace=True)
🎯 Variable Identification
Type	Also Called	Use In Model
Independent Variable (IV)	Feature	Input
Dependent Variable (DV)	Target	Output

Example:

Feature	Feature	Feature	Target
Salary	City	Experience	Purchase Decision

## 📈 Univariate Analysis
👉 Analysis of one variable at a time

python
Copy code
import seaborn as sns
sns.histplot(df['Age'])
Use for:

Frequency

Spread

Outliers

## 🔗 Bivariate Analysis
👉 Analyze relationship between 2 variables

python
Copy code
sns.scatterplot(data=df, x='Age', y='Salary')
Correlation

python
Copy code
sns.heatmap(df.corr(), annot=True)
Correlation Value	Meaning
+1	Strong positive
0	No correlation
-1	Strong negative

## 🚨 Outlier Detection / Anomaly Detection
Outlier impacts ML models like:

Logistic Regression

KNN

python
Copy code
sns.boxplot(df['Salary'])
Treatment:

IQR Method

Winsorization

Log Transform

## 🔠 Variable Creation — Encoding
Machine does not understand:

Copy code
Sunny, Winter, Rainy
Convert using dummy variables:

python
Copy code
df = pd.get_dummies(df, columns=['Season'], drop_first=True)
🛠 Tools Used
Category	Tools
Data Handling	Pandas, NumPy
Visualization	Matplotlib, Seaborn
ML Modeling	Scikit-Learn
Dashboard (Optional)	Tableau / Power BI
IDE / Notebook	Jupyter / VS Code

## 🧪 Practical EDA Workflow
Step	Description
- 1️⃣ Load Data	CSV / Excel
- 2️⃣ Inspect	df.head(), df.info()
- 3️⃣ Clean Data	Missing value treatment
- 4️⃣ Transform	Type conversion & encoding
- 5️⃣ Detect Outliers	Boxplots, stats
- 6️⃣ Feature Insights	EDA charts
- 7️⃣ Save Clean Dataset	Use for model training
