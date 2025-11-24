# 🚢 Titanic – Data Cleaning & Exploratory Data Analysis (EDA)

## **📌 Project Overview**
This project performs **data cleaning** and **exploratory data analysis (EDA)** on the Titanic dataset.  
It includes interactive visualizations, structured analysis, and a final business insights report.

This repository is part of an internship submission task.

---

## 📁 **Repository Structure**
```
Titanic-EDA-and-Data-Cleaning/
│
├── data/
│   ├── train.csv                    → Original raw dataset
│   └── cleaned_titanic.csv          → Cleaned dataset used for analysis
│
├── notebooks/
│   ├── Cleaning_Train_dataset.ipynb → Data inspection + cleaning
│   ├── Titanic_dataset_EDA.ipynb    → Full EDA with Plotly visuals
│   ├── Cleaning_Train_dataset.html  → Optional HTML export
│   └── Titanic_dataset_EDA.html     → Optional HTML export
│
├── reports/
│   └── Titanic_EDA_Insights_Report.pdf → Final business insights summary
│
└── README.md
```

---

## 🧹 **Data Cleaning Summary**

Cleaning performed inside:  
**`notebooks/Cleaning_Train_dataset.ipynb`**

### ✔ Steps Completed:
- Dataset inspection:
  - `df.shape`, `df.info()`, `df.describe()`
  - Missing value check  
  - Duplicate detection
- Missing value handling:
  - **Age** → replaced with median  
  - **Embarked** → replaced with mode  
  - **Cabin** → replaced with `"Unknown"`
- Removed unnecessary spaces from string columns  
- Checked and corrected data types  
- Exported cleaned dataset as **cleaned_titanic.csv**

---

## 📊 **Exploratory Data Analysis (EDA)**

EDA is performed in:  
**`notebooks/Titanic_dataset_EDA.ipynb`**

### 🔍 Visuals Included

#### 🔹 **Univariate Analysis**
- Histogram → Age Distribution  
- Bar Chart → Gender Distribution  

#### 🔹 **Bivariate Analysis**
- Grouped Bar Chart → Survival by Gender  
- Box Plot → Fare vs Survival  

#### 🔹 **Multivariate Analysis**
- Correlation Heatmap (numeric features)  
- Scatter Plot → Age vs Fare colored by Survival  

All charts built using **Plotly** with **clean pastel colors** and **interactive tooltips**.

---

## 📌 **Key Insights (Business Perspective)**

### 🧍 Passenger Demographics
- Most passengers fall in the **20–40 age group**  
- Gender distribution:
  - **Male:** ~65%  
  - **Female:** ~35%

---

### 🛟 Survival Insights
- **Female survival rate:** ~75%  
- **Male survival rate:** ~20%  
➡️ Gender is the **strongest driver** of survival.

---

### 💰 Fare & Class Patterns
- Survivors generally paid **higher fares**
- **1st class** passengers had significantly higher survival  
- **3rd class** passengers had the **highest non-survival count**  
➡️ Socio-economic status strongly influenced survival outcomes

---

### 📈 Correlation Findings
- **Positive correlation** → Fare & Survival  
- **Negative correlation** → Pclass & Survival  
- Age, SibSp, Parch → weak correlation with survival  

---

### 📝 Overall Summary
Survival was impacted mainly by:
- Evacuation rules (*women and children first*)
- Class-based accessibility  
- Lifeboat proximity  

A fully detailed explanation is available in:  
📄 **`reports/Titanic_EDA_Insights_Report.pdf`**

---

## 🛠️ **Tech Stack Used**
- **Python 3**
- **Pandas, NumPy** → data processing  
- **Plotly Express** → interactive visualizations  
- **Jupyter Notebook** → analysis environment  

---

## ▶️ **How to Run This Project**

### **1️⃣ Clone the repository**
```bash
git clone https://github.com/<your-username>/Titanic-EDA-and-Data-Cleaning.git
cd Titanic-EDA-and-Data-Cleaning
```

### **2️⃣ Install dependencies**
```bash
pip install pandas numpy plotly jupyter
```

### **3️⃣ Launch Jupyter Notebook**
```bash
jupyter notebook
```

### **4️⃣ Open the notebooks**

**Data Cleaning:**  
`notebooks/Cleaning_Train_dataset.ipynb`

**EDA:**  
`notebooks/Titanic_dataset_EDA.ipynb`

---

## 🎯 **Conclusion**

This project demonstrates:

- ✔ End-to-end **data cleaning**
- ✔ Structured **EDA workflow**
- ✔ Interactive **visual storytelling**
- ✔ Business-focused **insights & findings**
- ✔ Professional documentation with a PDF report

This repository showcases strong foundational skills essential for **data analytics roles and internships**.

---
