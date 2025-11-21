# 📊 Exploratory Data Analysis (EDA) — 7 Core Techniques

Exploratory Data Analysis (**EDA**) is the process of examining a dataset to **summarize its main characteristics**, identify patterns, detect anomalies, and test assumptions before building any machine learning model.  
It helps us **understand the data** better and decide the right preprocessing and modeling techniques.

---

## 🔍 1️⃣ Variable Identification
Classifying the dataset variables based on their types:

| Type | Examples | Description |
|------|-----------|-------------|
| **Categorical** | Gender, Country | Non-numerical labels |
| **Numerical** | Age, Salary | Measurable values |
| **Ordinal** | Ratings (1–5) | Ordered categories |
| **Date/Time** | Timestamp | Time-based features |
| **Text** | Comments, Address | Free-form strings |

---

## 📈 2️⃣ Univariate Analysis
Analyzing each variable **individually** to understand its distribution.

📌 Common Techniques:
- Frequency tables (Categorical)
- Histograms
- Box Plots
- Count Plots
- Summary statistics (mean, median, mode, variance)

---

## 🔗 3️⃣ Bivariate Analysis
Understanding the **relationship between two variables**.

📌 Common Techniques:
- Scatter Plot → Numerical vs Numerical
- Heatmap → Correlation
- Bar Plot → Categorical vs Numerical
- Crosstab / Chi-Square Test → Categorical vs Categorical

---

## 🚨 4️⃣ Outlier Detection
Finding extreme values that may impact the model performance.

📌 Common Techniques:
- Box plot (IQR rule: Q3 + 1.5×IQR)
- Z-Score (|Z| > 3)
- Scatter plots for visual identification
- Domain knowledge

---

## 🧩 5️⃣ Missing Value Imputation
Handling **missing or NULL** values in the dataset.

📌 Methods:

| Variable Type | Technique |
|--------------|-----------|
| Numerical | Mean / Median / KNN Imputation |
| Categorical | Mode / Most Frequent category |
| Time Series | Forward fill / Backward fill |
| Predictive | Models to estimate missing values |

---

## 🧪 6️⃣ Feature Engineering
Creating **new meaningful features** from existing ones to improve model performance.

Examples:
- Extracting year/month from date
- Binning continuous data (e.g., Age groups)
- Encoding categorical variables (One-Hot Encoding)
- Log transformation to reduce skewness

---

## ⚙️ 7️⃣ Feature Scaling
Ensuring numerical values remain **on the same scale**.

📌 Techniques:
- Standardization (Z-Score Scaling)
- Min-Max Scaling
- Robust Scaling (better for outliers)
- Normalization (L2 norm)

---

### 🎯 Final Note
EDA is a crucial step in every Data Science project.  
The better you explore the data, the better your ML model performs! 🚀  

---

### ⭐ Support
If you found this helpful, give it a ⭐ on GitHub and continue exploring datasets!

---
