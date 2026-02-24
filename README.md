# 📊 Hiring Process Analytics — Excel Data Analysis Project

> Analyzed 7,167 hiring records from a simulated multinational company dataset to uncover gender distribution, salary patterns, departmental composition, and position tier breakdown using Excel.

---

## 📌 Project Overview

This project simulates the role of a **Data Analyst at a multinational company (Google-scale)**. The task was to analyze historical hiring data and extract meaningful insights that can help the HR department improve decision-making around recruitment, salary benchmarking, and workforce composition.

**Tools Used:** Microsoft Excel (COUNTIFS, AVERAGE, MEDIAN, Pivot Tables, Charts)
**Dataset Size:** 7,167 records | 7 columns
**Skills Demonstrated:** Data Cleaning, Statistical Analysis, Salary Distribution, Pivot Tables, Data Visualization

---

## 📁 Workbook Structure

| Sheet | Task | Purpose |
|---|---|---|
| `Table1` | Raw Data | Original dataset — 7,167 hiring records |
| `Q1` | Hiring Analysis | Gender distribution of hired employees |
| `Q2` | Salary Analysis | Average, median, min, max, std deviation |
| `Q3` | Salary Distribution | Class intervals and histogram |
| `Q4` | Departmental Analysis | Headcount by department with chart |
| `Q5` | Position Tier Analysis | Distribution across position tiers |

---

## 📊 Dataset Description

| Column | Description |
|---|---|
| `application_id` | Unique identifier for each applicant |
| `Interview Taken on` | Date and time of interview |
| `Status` | Outcome — Hired or Rejected |
| `Gender` | Applicant gender |
| `Department` | Department applied to |
| `Post Name` | Position tier code (e.g. c5, i7, b9) |
| `Offered Salary` | Salary offered to the applicant (₹) |

---

## 🔎 Task A — Hiring Analysis: Gender Distribution

**Question:** How many males and females have been hired by the company?

**Filter Applied:** Status = Hired only (4,697 total hired out of 7,167 applicants)

| Gender | Hired Count |
|---|---|
| Male | 2,563 |
| Female | 1,856 |
| Don't Want to Say | 268 |
| Unknown | 10 |
| **Grand Total** | **4,697** |

**Insight:** Males account for approximately 55% of hires, females 39%. The 6% gap suggests a moderate gender imbalance in hiring outcomes that warrants further investigation across departments and roles.

---

## 💰 Task B — Salary Analysis

**Question:** What is the average salary offered by this company?

| Metric | Value |
|---|---|
| Average Salary | ₹49,983 |
| Median Salary | ₹49,625 |
| Minimum Salary | ₹100 |
| Maximum Salary | ₹4,00,000 |
| Total Salary Paid | ₹35,82,28,369 |
| Std Deviation | ₹28,854 |

**Insight:** The average (₹49,983) and median (₹49,625) are very close, indicating a relatively balanced salary distribution. However, the wide range from ₹100 to ₹4,00,000 and a standard deviation of ₹28,854 highlights significant variation across roles and seniority levels.

---

## 📊 Task C — Salary Distribution: Class Intervals

**Question:** Create class intervals to understand salary distribution across the workforce.

**Method:** COUNTIFS formula applied against salary column across 7 defined bands.

| Salary Range | Employee Count |
|---|---|
| ₹0 – ₹50,000 | Majority (~53%) |
| ₹50,001 – ₹1,00,000 | Mid segment |
| ₹1,00,001 – ₹1,50,000 | Smaller group |
| ₹1,50,001 – ₹2,00,000 | Declining |
| ₹2,00,001 – ₹2,50,000 | Small |
| ₹2,50,001 – ₹3,00,000 | Very small |
| ₹3,00,001 – ₹4,00,000 | Outlier range |

**Insight:** The salary distribution is right-skewed — the majority of employees earn below ₹50,000, with a small group of high earners pulling the average upward. This is typical of large organizations with a broad base of entry and mid-level roles.

---

## 🏢 Task D — Departmental Analysis

**Question:** What is the proportion of people working in different departments?

| Department | Headcount | % of Total |
|---|---|---|
| Operations | 2,771 | 38.7% |
| Service | 2,055 | 28.7% |
| Sales | 746 | 10.4% |
| Production | 380 | 5.3% |
| Purchase | 333 | 4.6% |
| Marketing | 325 | 4.5% |
| Finance | 288 | 4.0% |
| General Management | 172 | 2.4% |
| Human Resources | 97 | 1.4% |
| **Grand Total** | **7,167** | **100%** |

**Insight:** Operations (39%) and Service (29%) together account for nearly 68% of the entire workforce — indicating a heavily operations-driven organization. HR and General Management are significantly underrepresented relative to total headcount, which may suggest lean corporate functions typical of large-scale service companies.

---

## 📈 Task E — Position Tier Analysis

**Question:** What is the distribution of employees across different position tiers?

| Position Code | Count | Tier Type |
|---|---|---|
| c9 | 1,792 | Clerical |
| c5 | 1,747 | Clerical |
| i7 | 981 | Intermediate |
| i5 | 787 | Intermediate |
| b9 | 463 | Basic |
| i6 | 527 | Intermediate |
| c8 | 320 | Clerical |
| c-10 | 232 | Clerical |
| i1 | 222 | Intermediate |
| i4 | 88 | Intermediate |
| m6, m7 | 4 | Management |
| n6, n9, n10 | 3 | Senior/Executive |
| **Grand Total** | **7,167** | |

**Insight:** Clerical positions (c-tier) dominate at nearly 57% of the workforce, followed by intermediate roles (i-tier) at 36%. Management (m-tier) and senior/executive (n-tier) positions represent less than 0.1% of total headcount — consistent with a large pyramid-shaped organizational structure typical of multinational companies.

---

## 🛠️ Data Cleaning Notes

- **Missing Values:** 1 record had a missing Post Name — retained as it did not affect salary or department analysis
- **Outliers Identified:** Minimum salary of ₹100 flagged as a potential data entry error. Maximum of ₹4,00,000 retained as it represents senior-level compensation
- **Gender Standardization:** "Unknown" and "Don't want to say" treated as separate valid categories rather than nulls
- **Status Filter:** Tasks A–E focused on all 7,167 records; gender hire analysis filtered to Hired status (4,697 records)

---

## 💡 Key Takeaways

1. **Gender gap exists** — Males hired at 55% vs females at 39% among confirmed hires
2. **Salary is balanced at mid-level** — Average and median within ₹400 of each other, but outliers at both ends are wide
3. **Operations-heavy workforce** — Two departments alone account for 68% of all employees
4. **Pyramid-shaped hierarchy** — Clerical and intermediate tiers dominate; management roles are extremely rare
5. **Salary distribution is right-skewed** — Majority earn below ₹50,000, small high-earner group pulls average up

---

## 🔗 Connect

**LinkedIn:** [linkedin.com/in/guptaharsh1401](https://linkedin.com/in/guptaharsh1401)
**GitHub:** [github.com/Harsh1887](https://github.com/Harsh1887)
