# 📊 Employee Data Analysis Project (Python)

## 🏢 Project Overview
This project was completed as part of the **SkilloVilla Data Analytics Program (February 2026)**. It focuses on analyzing employee, project, and organizational hierarchy data using Python.

The goal was to transform multiple datasets into a structured and easy-to-navigate format while extracting meaningful business insights.

---

## 🎯 Problem Statement

Organizations operating across multiple international cities needed a **single refined dataset** combining:

- Employee details
- Project assignments
- Seniority levels

The challenge was to:
- Merge multiple datasets
- Handle missing values
- Analyze project ownership
- Calculate total project costs per employee

---

## 🧠 Key Objectives

- Link multiple datasets using a unique ID
- Identify employees responsible for projects
- Map employees to their seniority levels
- Calculate total cost of projects per employee
- Clean and transform raw data

---

## 🛠️ Tools & Technologies

- Python 🐍
- Pandas
- NumPy
- Jupyter Notebook

---

## ⚙️ Project Workflow

### 1. Data Creation
- Created three DataFrames:
  - Employee Data
  - Project Data
  - Seniority Level Data
- Exported them as `.csv` files

### 2. Data Cleaning
- Handled missing values in project cost
- Replaced missing values using **running average**

### 3. Data Transformation
- Split full names into:
  - First Name
  - Last Name
- Removed unnecessary columns
- Added prefixes (Mr./Mrs.)

### 4. Data Integration
- Merged all three datasets into one **Final DataFrame**

### 5. Feature Engineering
- Added:
  - Bonus column (5% for completed projects)
  - Updated designation levels
  - Promotions/demotions based on conditions

### 6. Analysis
- Calculated **total project cost per employee**
- Filtered employees based on city conditions

---

## 📈 Key Insights

- Identified employee contribution across multiple projects
- Mapped project ownership with hierarchy
- Evaluated employee performance via project success/failure
- Calculated total financial impact per employee

---

## 📊 Project Structure

employee-data-analysis-python/
│
├── data/
│ ├── employee.csv
│ ├── project.csv
│ ├── seniority.csv
│
├── notebooks/
│ └── employee_analysis.ipynb
│
├── output/
│ └── final_dataset.csv
│
├── README.md
└── requirements.txt


---

## 📌 Sample Code Snippet

```python
import pandas as pd
import numpy as np

# Load datasets
employee = pd.read_csv('employee.csv')
project = pd.read_csv('project.csv')
seniority = pd.read_csv('seniority.csv')

# Merge datasets
final = pd.merge(employee, project, on='ID')
final = pd.merge(final, seniority, on='ID')

# Fill missing values
project['Cost'] = project['Cost'].fillna(project['Cost'].mean())
```

### 🚀 Results

**Successfully merged and cleaned** multiple datasets

**Built a structured and analysis**-ready dataset

**Demonstrated strong skills in:**

*Data manipulation*

*Data cleaning*

*Python programming*

✅ Achieved 100% project completion

---

### 📚 Learnings

Real-world data handling using Pandas

Data transformation techniques

Feature engineering

Business-focused data analysis

---
### 👩‍💻 Author

## Drakshayani

Aspiring Data Analyst | Python | Data Analytics

---
⭐ If you like this project

Give it a ⭐ on GitHub!
---
### links:

numpy[Capstone project - Python Fundamentals (2).pdf](https://github.com/user-attachments/files/26169010/Capstone.project.-.Python.Fundamentals.2.pdf)

jupyter[PYTHON ANSWERKEY.ipynb](https://github.com/user-attachments/files/26169003/PYTHON.ANSWERKEY.ipynb)

