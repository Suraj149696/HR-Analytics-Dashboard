<div align="center">

<!-- HEADER BANNER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4F46E5,100:7C3AED&height=200&section=header&text=HR%20Analytics%20Dashboard&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Workforce%20Intelligence%20%7C%20Attrition%20Analysis%20%7C%20Power%20BI&descSize=16&descAlignY=58&descColor=c7d2fe" width="100%"/>

<!-- BADGES -->
<p>
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI"/>
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white" alt="Excel"/>
  <img src="https://img.shields.io/badge/DAX-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="DAX"/>
  <img src="https://img.shields.io/badge/HR%20Analytics-4F46E5?style=for-the-badge&logo=databricks&logoColor=white" alt="HR Analytics"/>
  <img src="https://img.shields.io/badge/Status-Complete-22c55e?style=for-the-badge" alt="Complete"/>
</p>

<br/>

> **Turning raw HR data into strategic workforce decisions** — an end-to-end Power BI solution that identifies why employees leave and what leadership can do about it.

<br/>

</div>

---

## 📌 Project Overview

A comprehensive **HR Analytics Dashboard** built to help organisations **reduce employee attrition**, improve workforce retention, and make data-driven HR decisions. The dashboard transforms raw HR data into clear, actionable visual intelligence — surfacing the hidden patterns behind employee turnover.

This project replicates a real-world **HR Business Analyst** workflow:

- ✅ Raw data ingestion, cleaning & validation
- ✅ Feature engineering and DAX-powered KPIs
- ✅ Interactive Power BI dashboard for HR leaders
- ✅ Attrition drivers identified with visual evidence
- ✅ Actionable recommendations for talent retention

---

## 📊 Dashboard Preview

<div align="center">
<img src="Hr Dashboard.png" width="90%" style="border-radius:10px;" alt="HR Analytics Dashboard Preview"/>
<br/>
<sub><i>Interactive Power BI Dashboard — Attrition, Demographics & Performance Analysis</i></sub>
</div>

---

## 🎯 Business Problem

> **"Why are our best employees leaving — and how do we stop it?"**

High employee attrition is costly. Replacing a single employee can cost **50–200% of their annual salary** when factoring in recruitment, onboarding, and lost productivity. This dashboard gives HR professionals a single source of truth to answer:

- Which departments have the **highest attrition rates**?
- What **age groups and job roles** are most at risk?
- Does **salary, education, or tenure** predict turnover?
- Where should HR focus **retention efforts first**?

---

## 🔑 Key Insights Delivered

| Insight Area | What the Dashboard Reveals |
|---|---|
| 📉 **Attrition Rate** | Overall attrition % with trend over time |
| 👥 **By Department** | Which teams are losing the most talent |
| 🎂 **By Age Group** | Identifies at-risk age brackets |
| 💼 **By Job Role** | Roles with highest turnover frequency |
| 💰 **By Salary Slab** | Correlation between pay band and attrition |
| 🎓 **By Education** | Education field vs attrition relationship |
| 📅 **By Years at Company** | Tenure-based attrition patterns |

---

## 🛠️ Workflow — Step by Step

```
Raw HR Data (CSV)
      │
      ▼
 ┌─────────────────────┐
 │  1. Data Cleaning   │  ← Excel: nulls, duplicates, type fixes
 └─────────┬───────────┘
           │
           ▼
 ┌──────────────────────────┐
 │  2. Data Transformation  │  ← Binning age/salary, encoding categories
 └─────────┬────────────────┘
           │
           ▼
 ┌──────────────────────────┐
 │  3. Power BI Modelling   │  ← Relationships, DAX measures, KPIs
 └─────────┬────────────────┘
           │
           ▼
 ┌──────────────────────────┐
 │  4. Dashboard Design     │  ← Interactive visuals, slicers, drill-down
 └─────────┬────────────────┘
           │
           ▼
 ┌──────────────────────────┐
 │  5. Insights & Actions   │  ← Attrition root causes + HR recommendations
 └──────────────────────────┘
```

---

## 📁 Repository Structure

```
HR-Analytics-Dashboard/
│
├── 📊  HR Dashboard.pbix        ← Power BI dashboard (main deliverable)
├── 📄  HR_Analytics.csv         ← Source dataset
├── 🖼️  Hr Dashboard.png         ← Dashboard screenshot
└── 📝  README.md
```

---

## ⚙️ Tools & Technologies

<div align="center">

| Tool | Purpose |
|---|---|
| ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black) | Dashboard design, DAX measures, interactive reporting |
| ![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoft-excel&logoColor=white) | Data cleaning, preprocessing, validation |
| **DAX** | Calculated columns, KPI measures, dynamic filtering |
| **Power Query** | Data transformation pipeline inside Power BI |

</div>

---

## 💡 Key DAX Measures Used

```dax
-- Attrition Rate
Attrition Rate = 
DIVIDE(
    COUNTROWS(FILTER('HR_Analytics', 'HR_Analytics'[Attrition] = "Yes")),
    COUNTROWS('HR_Analytics'),
    0
)

-- Active Employees
Active Employees = 
COUNTROWS(FILTER('HR_Analytics', 'HR_Analytics'[Attrition] = "No"))

-- Average Age
Avg Age = AVERAGE('HR_Analytics'[Age])
```

---

## 🚧 Challenges & How I Solved Them

| Challenge | Approach |
|---|---|
| **Incomplete / dirty data** | Applied Excel-based validation rules; removed nulls and outliers before import |
| **Complex visualisation logic** | Used DAX conditional measures and custom calculated columns for accurate segmentation |
| **Making it usable for non-technical HR teams** | Focused on clean layout, plain-language labels, and interactive slicers requiring zero training |

---

## 📈 Business Impact

- 🔍 **Root causes** of attrition identified across salary, tenure, role, and department dimensions  
- 🎯 HR teams can now **prioritise at-risk employee segments** rather than using guesswork  
- 📋 Dashboard replaces **manual Excel reporting**, saving hours of weekly analysis  
- 💬 Findings provide a **data-backed brief** for compensation reviews and engagement programmes

---

## 🚀 How to Use

```bash
# 1. Clone the repository
git clone https://github.com/Suraj149696/HR-Analytics-Dashboard.git

# 2. Open the dataset (optional review)
#    HR_Analytics.csv — open in Excel or any CSV viewer

# 3. Open the dashboard
#    Open HR Dashboard.pbix in Microsoft Power BI Desktop

# 4. Explore
#    Use slicers to filter by department, job role, age group, salary slab
```

> **Requirement:** [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free) — available for Windows.

---

## 📬 Connect with Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Suraj%20Jagtap-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/suraj-jagtap-data-analyst/)
[![GitHub](https://img.shields.io/badge/GitHub-Suraj149696-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Suraj149696)
[![Email](https://img.shields.io/badge/Email-suraj149696%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:suraj149696@gmail.com)

<br/>

*Open to roles: Data Analyst · HR Analytics · Business Analyst · MIS Analyst*

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7C3AED,100:4F46E5&height=100&section=footer" width="100%"/>

<sub>Built with Power BI · Excel · DAX &nbsp;|&nbsp; Suraj Jagtap &nbsp;|&nbsp; 2024</sub>

</div>
