
# 📊 Customer Personality Analysis — Task 1

### 🧠 Internship Project: Data Cleaning & Preprocessing

This repository contains the cleaned dataset and Python script used for **Task 1** of the **Data Analyst Internship**. The objective was to clean and prepare the raw *Customer Personality Analysis* dataset for further analysis or modeling.

---

### ✅ Task Objective

Clean and preprocess the raw dataset by addressing:
- Missing values
- Duplicate records
- Inconsistent formatting (text/date)
- Standardizing column names and data types

---

### 🧰 Tools Used

- **Python**: Data processing
- **Pandas**: Data manipulation
- **Seaborn & Matplotlib**: Data visualization
- **Jupyter Notebook**

---

### 📂 Files in This Repository

| File Name | Description |
|-----------|-------------|
| `marketing_campaign.csv` | Original dataset from Kaggle |
| `cleaned_marketing_campaign.csv` | Final cleaned dataset |
| `data_cleaning_script.py` | Python script for cleaning |
| `README.md` | Task summary and documentation |

---

### 🔧 Cleaning Steps Performed

- ✅ Removed rows with missing `Income` values
- ✅ Dropped duplicate records
- ✅ Standardized categorical fields: `Gender`, `Marital_Status`, `Education`
- ✅ Converted `Dt_Customer` to datetime format
- ✅ Renamed columns to lowercase and used snake_case format
- ✅ Derived `Age` column from `Year_Birth`
- ✅ Converted data types (e.g., `Income` to float)
- ✅ Removed outliers in `Income` using 99th percentile filtering

---

### 📌 Sample Code Snippet

```python
df['Dt_Customer'] = pd.to_datetime(df['Dt_Customer'], format='%d-%m-%Y')
df.columns = df.columns.str.strip().str.lower().str.replace(' ', '_')
df['age'] = 2025 - df['year_birth']
```

---

### 📤 Submission Guidelines Followed

- 🗃️ GitHub Repo with code, cleaned dataset, and README
- ⏳ Task completed within submission time window
- 📚 Used only free, open-source tools

---

### 🙋‍♂️ About Me

**Name**: Uttam Mehta  
**Role**: Data Analyst Intern  
