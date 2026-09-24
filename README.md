# Railway Operations Intelligence & Delay Root-Cause Analytics

## 📌 Project Overview

An end-to-end Data Analytics project analyzing 1.5 million railway journeys to identify delay patterns, operational bottlenecks, seasonal risks, train-type performance, and major delay causes.

The project uses Python, SQL (DuckDB), and Excel to transform raw railway operations data into actionable business insights.

---

## 🎯 Business Objective

The objective is to understand:

- Which railway zones experience the highest delays?
- Which train types have higher delay rates?
- How does seasonality affect delays?
- Does a late incoming rake increase the probability of delay?
- What are the major recorded causes of delays?
- Which zone–train combinations require operational attention?
- What actions can management take to reduce severe delays?

---

## 📊 Dataset

- Records: 1.5 million journeys
- Features: 45
- Period: 2018–2024
- Missing values: 0
- Duplicate records: 0

The dataset contains operational attributes such as:

- Railway zone
- Train type
- Delay minutes
- Delay status
- Weather/fog indicators
- Monsoon indicators
- Late incoming rake
- Track congestion
- Maintenance indicators
- Distance
- Coach and locomotive age
- Delay causes

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQL
- DuckDB
- Excel
- Statistical Analysis

---

## 🔎 Project Workflow

### 1. Data Loading
Loaded the railway operations dataset using Pandas.

### 2. Data Quality Audit
Checked:

- Missing values
- Duplicate records
- Invalid values
- Data types
- Date ranges
- Outliers and data consistency

### 3. Data Cleaning
Validated delay minutes, departure hours, months, railway zones, and other operational fields.

### 4. Feature Engineering

Created:

- Delay categories
- Route proxy
- Seasonal indicators
- Operational risk indicators

### 5. SQL Analysis

Used DuckDB SQL to analyze:

- Zone performance
- Train-type performance
- Monthly trends
- Delay causes
- Late incoming rake
- Fog risk
- Zone × train-type combinations

### 6. Statistical Analysis

Performed:

- Correlation analysis
- Chi-square test
- Confidence interval analysis

### 7. Excel Dashboard

Created a management-oriented Control Tower containing:

- KPI summary
- Zone Performance
- Route Intelligence
- Time Intelligence
- Root Cause Analysis
- Action Matrix
- Scenario Analysis

---

## 📈 Key Insights

1. Overall delay rate was **71.89%** across 1.5 million journeys.

2. **Eastern Railway (ER)** had the highest zone-level delay rate at **89.32%**.

3. **South Western Railway (SWR)** had the lowest delay rate at **50.22%**.

4. Monsoon-period journeys had a delay rate of **92.82%**, compared with **61.40%** outside the monsoon period.

5. Passenger Trains had an **88.04%** delay rate, while Vande Bharat had **44.34%**.

6. Journeys with a late incoming rake had an **87.05%** delay rate compared with **63.75%** when the rake was not late.

7. The two largest recorded delay causes were **Track Congestion (22.41%)** and **Flooding/Waterlogging (19.37%)** among delayed journeys.

8. Delay patterns appear to be influenced by multiple operational and environmental factors rather than a single cause.

---

## 📁 Project Files

```text
Railway-Operations-Analytics/
│
├── Railway_Operations_Analytics.ipynb
├── README.md
│
├── data/
│   └── railway_operations.csv
│
├── outputs/
│   ├── charts/
│   └── analysis_outputs/
│
└── dashboard/
    └── RailOps_Control_Tower.xlsx
