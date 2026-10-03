# 📊 Jobs Salary Dashboard (Microsoft Excel)

![Jobs Salary Dashboard](images/ExcelDashbord.png)

An interactive Excel dashboard that analyzes **32,672 data and tech job postings from 2023 across 111 countries**. Pick a job title, country, and job type, and every KPI and chart updates to show salary ranges, pay by role, pay by employment type, and how salaries vary around the world.

---

## 📌 Overview

| | |
|---|---|
| **Tool** | Microsoft Excel (Microsoft 365) |
| **Dataset** | 32,672 job postings, Jan to Dec 2023 |
| **Coverage** | 111 countries, 10 job titles |
| **Output** | Single page interactive dashboard |

**Questions it answers**
- How many postings exist for a given role, and what is the salary range?
- Which roles pay the most in a selected country?
- How does pay differ between full-time, part-time, contract, and temp work?
- Which countries pay the most for a selected role?

---

## 🎯 Dashboard Features

### Interactive Selectors

<p align="center">
  <img src="images/Slicers.png" alt="Selectors" width="1000">
</p>

Three dropdown selectors at the top drive the whole dashboard:

- **Job Title:** Data Analyst, Data Scientist, Data Engineer, Business Analyst, Machine Learning Engineer, Software Engineer, Cloud Engineer, and senior variants
- **Country:** any of the 111 countries in the dataset
- **Job Type:** Full-time, Part-time, Contractor, Temp work

### 📈 KPI Cards

- **Job Count:** number of postings for the selection
- **Min Salary:** lowest yearly salary
- **Max Salary:** highest yearly salary

### 📊 Visuals

| Visual | What it shows |
|--------|---------------|
| **Job Category** bar chart | Median yearly salary for every job title in the selected country, with the selected title highlighted |
| **Job Type** bar chart | Median yearly salary by employment type, with the selected type highlighted |
| **World Map** | Filled map of median salary by country for the selected role |

---

## 🗂️ Dataset

Source file: `source/Jobs Data.xlsx` (one row per posting)

| Column | Description |
|--------|-------------|
| `job_title_short` | Standardized job title (10 categories) |
| `job_title` | Original posting title |
| `job_country` | Country of the job |
| `job_schedule_type` | Employment type (Full-time, Contractor, Part-time, etc.) |
| `job_work_from_home` | Remote flag |
| `job_posted_date` | Posting date (2023) |
| `salary_rate` | Yearly or hourly |
| `salary_year_avg` / `salary_hour_avg` | Salary values |
| `company_name` | Hiring company |
| `job_skills` | Skills listed in the posting |
| `job_via` | Platform the job was posted on |

---

## 🧹 Data Preparation

- Converted the raw data into a structured Excel Table for dynamic references
- Grouped 26 mixed schedule values (for example, "Full-time and Part-time") into four clean job types
- Used yearly salary as the main measure for consistent comparisons
- Built a list of unique titles, countries, and job types to feed the dropdowns

---

## 🛠️ Excel Features Used

- **Data Validation** dropdowns as dashboard selectors
- **Named ranges** for selector values
- **Dynamic formulas** that recalculate KPIs and chart data from the selections
- **Bar charts** with conditional highlighting of the selected item
- **Filled Map chart** for geographic salary comparison
- **KPI cards** and a clean single page layout
- **Sheet protection** so users can only change the selectors

---

## 📂 Repository Structure

```
Excel-jobs-sales-dashbord/
├── final/
│   └── Jobs Data Final.xlsx     # Finished dashboard workbook
├── source/
│   └── Jobs Data.xlsx           # Raw job postings data
├── images/
│   ├── ExcelDashbord.png        # Dashboard screenshot
│   └── Slicers.png              # Selector close up
├── LICENSE
└── README.md
```

---

## 🚀 How to Use

1. Download `final/Jobs Data Final.xlsx`
2. Open it in Excel for Microsoft 365 (needed for the Map chart and dynamic array formulas)
3. Use the three dropdowns at the top to pick a job title, country, and job type
4. Read the KPIs and charts as they update

---

## 💡 Skills Demonstrated

Advanced Excel · Dashboard Design · Data Cleaning · Dynamic Formulas · Data Validation · Data Visualization · Map Charts · Business Reporting

---

## 📄 License

MIT License. See `LICENSE` for details.

---

## 👤 About Me

**Abdul Moiz Waheed**
Data Analyst and Analytics Engineer working with SQL Server, Power BI, Excel, and Python.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/abdul-moiz-s2402)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MoizWaheed80)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:moizwaheed80@gmail.com)
