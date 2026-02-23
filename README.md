# 📊 Hiring Process Analytics — Excel Data Analysis Project

## Project Overview
Analyzed a company's hiring dataset (7,141 records) to uncover trends in gender distribution, salary structure, departmental headcount, and position tiers. The goal was to help the HR/hiring team make data-driven decisions about workforce planning and compensation.

**Tools Used:** Microsoft Excel (Pivot Tables, VLOOKUP, Statistical Functions, Charts)  
**Dataset Size:** 7,141 applicant records | 7 columns  
**Skills Demonstrated:** Data Cleaning, Outlier Detection, Statistical Summarization, Data Visualization

---

## Dataset Description

| Column | Description |
|---|---|
| application_id | Unique applicant identifier |
| Interview Taken on | Date & time of interview |
| Status | Hired / Rejected |
| Gender | Applicant gender |
| Department | Department applied to |
| Post Name | Position tier code |
| Offered Salary | Salary offered (INR) |

---

## Tasks & Findings

### 1. 🧹 Data Cleaning & Handling Missing Values
- Identified **15 records** with "Unknown" gender and **392** marked "Don't want to say" — categorized separately rather than dropped to preserve data integrity
- Detected salary outliers (min: ₹100, max: ₹400,000) using IQR method; flagged extreme low values as data entry errors
- No duplicate application IDs found

### 2. 👥 A. Hiring Analysis — Gender Distribution

| Gender | Count |
|---|---|
| Male | 4,070 |
| Female | 2,664 |
| Don't want to say | 392 |
| Unknown | 15 |
| **Total Hired** | **4,679** |

**Insight:** Male hires outnumber female hires by ~53%. This gender gap may reflect broader applicant pool imbalances or department-level biases worth investigating further.

---

### 3. 💰 B. Salary Analysis — Average Salary

- **Average Salary Offered:** ₹50,009.96
- Calculated using Excel `AVERAGE()` function across all 7,140 valid salary records
- Median salary provides a better central tendency measure given outlier presence

---

### 4. 📊 C. Salary Distribution — Class Intervals

| Salary Range (₹) | Employee Count |
|---|---|
| 0 – 50,000 | ~3,800 |
| 50,001 – 100,000 | ~2,100 |
| 100,001 – 150,000 | ~800 |
| 150,001 – 200,000 | ~300 |
| 200,001+ | ~140 |

**Insight:** The majority of employees (~53%) fall in the ₹0–50K salary band, indicating a predominantly entry/mid-level workforce. A smaller proportion earns above ₹1.5L, representing senior/specialized roles.

---

### 5. 🏢 D. Departmental Analysis

| Department | Headcount |
|---|---|
| Operations Department | 2,762 |
| Service Department | 2,045 |
| Sales Department | 744 |
| Production Department | 379 |
| Purchase Department | 332 |
| Marketing Department | 325 |
| Finance Department | 287 |
| General Management | 171 |
| Human Resource Department | 96 |

**Insight:** Operations (39%) and Service (29%) departments account for nearly 68% of all hires — reflecting a heavily operations-driven organizational structure. HR is significantly understaffed relative to total headcount.

---

### 6. 🏷️ E. Position Tier Analysis

Position tiers follow a coding system (c = clerical, i = intermediate, b = business, m = management):

| Tier Code | Count | Tier Type |
|---|---|---|
| c9 | 1,783 | Clerical Senior |
| c5 | 1,743 | Clerical Mid |
| i7 | 977 | Intermediate Senior |
| i6 | 527 | Intermediate |
| b9 | 456 | Business Senior |
| i5 | 786 | Intermediate Mid |
| c8 | 319 | Clerical |
| c-10 | 232 | Clerical Top |
| i1 | 222 | Intermediate Entry |

**Insight:** Clerical and intermediate tiers dominate hiring volume. Management-level (m6, m7) hiring is minimal, consistent with a pyramid-shaped organizational hierarchy.

---

## Key Takeaways
1. Gender gap exists — male hires are ~53% of total; worth monitoring for equity
2. Average salary of ~₹50K masks significant variation; salary bands show most employees are entry-to-mid level
3. Operations and Service departments drive the majority of hiring demand
4. Workforce is predominantly clerical/intermediate tier — succession planning for senior roles may be needed

---
