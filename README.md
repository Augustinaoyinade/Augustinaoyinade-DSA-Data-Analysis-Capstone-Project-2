# Palmoria Group HR & Compensation Analysis  
A Gender-Focused Data Investigation for Equality, Compliance & Organizational Reform  
Powered by RetailTech Analytics

**Prepared for**: Mr. Yunus Shofoluwe, CHRO  
**By**: HR Analytics Consultant  
**Date**: July 2025  

---

##  Executive Summary

Palmoria Group, a manufacturing company in Nigeria operating in **Kaduna**, **Abuja**, and **Lagos**, is facing scrutiny following a media exposé titled **“Palmoria, the Manufacturing Patriarchy.”** The article has raised concerns about gender inequality, pay disparities, and performance evaluation bias. 

CHRO **Mr. Yunus Shofoluwe** has commissioned this report to identify core HR issues and provide data-driven recommendations.


## Project Overview

This project investigates employee demographic, performance, and compensation data from Palmoria to identify gender-based disparities, compliance breaches, and improvement opportunities. The analysis provides evidence-based insights and targeted recommendations to guide leadership in promoting fairness, trust, and equality.

---

## Data Source

Data was sourced from Palmoria’s internal HR system and analyzed using Power BI. It includes:

* **Employee Records**
  - Name
  - Department
  - Gender
  - Region
  - Salary
  - Rating

* **Bonus Rule Table**
  - Department
  - Rating thresholds
  - Corresponding bonus percentages

---

## Tools Used

* **Power BI Desktop**
  - Data transformation
  - Data modeling and integration
  - Dashboard creation for visual storytelling

* **DAX (Data Analysis Expressions)**
  - Used to calculate Bonus Amounts, Total Salary
* **Visualization Tools**
  - Stacked column chart
  - Stacked bar chart
  - 100% Stacked column chart
  - 100% Stacked bar chart
  - Clustered bar chart  
  - Clustered column chart  
  - Pie chart
  - Donut chart
  - Treemap
  - Area chart
  - Stacked area chaer
  - Cards

---

## Exploratory Data Analysis (EDA)

### Data Preparation
- Removed duplicate names
- Assigned generic gender status **(Dr)** with conditional column
- Removed blanks
- Removed NULL departments
- Changes datatypes as appropriate
- Create conditional column for SalaryBand (Grouped into $10,000 bands)
- Created derived columns:
  - `BonusAmount = Salary × BonusRate`
  - `TotalSalary = Salary + BonusAmount`
  

---

## Data Analysis


### 1. Gender Distribution Across Regions and Departments

###  Company-wide Totals:
- **Male**: 403 (51.2%)  
- **Female**: 374 (47.5%)  
- **Prefer Not to Say (Dr)**: 36 (1.3%)

### By Region:
| Region | Male | Female | Dr |
|--------|------|--------|----|
| Kaduna | 161  | 141    | 14 |
| Abuja  | 137  | 133    | 14 |
| Lagos  | 105  | 100    | 8  |

### By Department (%):
| Department            | Male     | Female   | Dr      |
|-----------------------|----------|----------|---------|
| Sales                 | 52.05%   | 42.47%   | 5.48%   |
| Product Management    | 52.00%   | 46.67%   | 1.33%   |
| Engineering           | 45.07%   | 47.89%   | 7.04%   |
| Legal                 | 56.34%   | 38.03%   | 5.63%   |
| Services              | 47.14%   | 50.00%   | 2.86%   |
| Human Resources       | 46.38%   | 49.28%   | 4.35%   |
| Support               | 53.63%   | 42.03%   | 4.35%   |
| Business Development  | 44.12%   | 51.47%   | 4.41%   |

> **Insight**: - Male over-representation is evident in **Legal**, **Sales**, and **Support**.
- Gender balance is closer in **Engineering, Services** and **Human Resources**.
- **Lagos** region shows the most equitable distribution.

### 2.  Performance Ratings by Gender

| Rating      | Male | Female | Dr |
|-------------|------|--------|----|
| Very Good   | 32   | 44     | 5  |
| Good        | 73   | 82     | 8  |
| Average     | 203  | 180    | 17 |
| Poor        | 64   | 49     | 3  |
| Very Poor   | 31   | 19     | 3  |

>  **Insight**: - **Female employees** are more likely to fall in the “Very Good” and “Good” categories.
- **Male employees** dominate “Poor” and “Very Poor” ratings. Indicates a need to review promotion and recognition frameworks to ensure high-performing female employees are being adequately advanced within the organization.

### 3. Salary Structure by Gender Distribution

### Total Salary Distribution:
- **Male**: $29.99M (49.87%)  
- **Female**: $27.25M (45.32%)  
- **Dr**: $2.89M (4.81%)

### Average Salary:
- **Male**: 32.7%  
- **Female**: 32.02%  
- **Dr**: 35.29%

### Departmental Disparities:
  - **Product Management, Sales, Legal,Engineering, Support** and  **Accounting** show considerable disparities with **Legal** and **Accounting** showing the greatest disparities


### Regional Pay Shares:
| Region | Male % | Female % | Dr % |
|--------|--------|----------|------|
| Kaduna | 50.94% | 44.30%   | 4.75%|
| Abuja  | 48.83% | 45.88%   | 5.29%|
| Lagos  | 49.67% | 46.06%   | 4.27%|

>  **Insight**:  **Average salaries appear close**, but gaps emerge when broken down by Sum of salary:
  -  **Department**: Largest in **Legal** and **Accounting**
  -  **Region**: Most disparities in **Kaduna**
-  Gender pay inequality is subtle but systemic.

### 4. Compliance with New $90,000 Regulation


- **Regulation**: Minimum $90,000 salary for all **manufacturing roles****.

- **Compliance**: Only 31.61% of manufacturing staff meet this threshold

>  **Insight**: High risk of **non-compliance penalties** and **reputation damage**, It poses legal risks. Immediate salary reviews are essential.

---

### 5. Salary Band Distribution

| Salary Band ($) | Employee Count |
|------------------|----------------|
| $10k–$20k        | 0              |
| $20k–$30k        | 23            |
| $30k–$40k        | 88            |
| $40k–$50k        | 88            |
| $50k–$60k        | 83            |
| $60k–$70k        | 82            |
| $70k–$80k        | 103          |
| $80k–$90k        | 89            |
| $90k–$100k      | 80            |
| $100k–$110k    | 93            |
| $110k–$120k    | 84            |

**Salary Band by Region**

| Salary Band ($) | Abuja | Kaduna | Lagos |
|------------------|--------|--------|--------|
| 20k–30k          | 6      | 12     | 5      |
| 30k–40k          | 34     | 36     | 18     |
| 40k–50k          | 36     | 29     | 23     |
| 50k–60k          | 29     | 38     | 16     |
| 60k–70k          | 30     | 30     | 22     |
| 70k–80k          | 30     | 41     | 32     |
| 80k–90k          | 31     | 33     | 25     |
| 90k–100k         | 27     | 29     | 24     |
| 100k–110k        | 36     | 35     | 22     |
| 110k–120k        | 25     | 33     | 26     |   


>  **Insight**: Most employees fall in the **$70k–$80k** range.
- A **significant portion** remains below $90k.
- **Kaduna** has the largest low-salary population showing regional disparity.

### 6. Bonus Allocation Based on Performance

**Bonus Policy Used:**

- Very Poor: 0.50%  
- Poor: 1.0 - 2.0%  
- Average: 2.0 - 4.0%
- Good: 4.1 -5.9%
- Very Good: 6.1 - 9.9%

**Total Bonus Amount**: $2,031,197.97

**Total Bonus by Region:**
- Kaduna: $763,606.85
- Abuja: $729,329.15
-Lagos: $538,261.97

**Total Salary (Bonus Inclusive):**
- Company-wide: $62,157,797.97

**Total Salary by Region:**
- Kaduna: $23,928,186.85
- Abuja: $21,416,739.15
-Lagos: $16,812,871.97

> **Insight**:  Bonuses align with ratings, **Kaduna** receives the largest bonus share  due to workforce size. However a fairness audit is recommended to avoid bias.

##  Recommendations

1. **Establish Gender Equity Frameworks**  
   - Create standardized guidelines for hiring, promotions, and salary reviews.  
   - Define and track measurable diversity key performance indicator across all departments.

2. **Conduct Department-Level Equity Reviews**  
   - Prioritize pay equity and performance evaluations in Legal and Accounting, where the most significant disparities exist.

3. **Ensure Compliance with Manufacturing Salary Regulations**  
   - Immediately review and adjust salaries for manufacturing staff earning below the $90,000 benchmark to meet regulatory standards.

4. **Invest in High-Performing Female Talent**  
   - Introduce mentorship programs, leadership training, and advancement opportunities for top-performing women to support retention and development.

5. **Monitor Progress Through Dashboards**  
   - Leverage Human Resources dashboards to track gender distribution, salary equality, and performance trends on an ongoing basis.

6. **Review Regional Bonus Allocation**  
   - Evaluate bonus distribution across regions to ensure fairness in relation to workforce size and performance contributions.

7. **Communicate Internally**
   - Share these findings internally and planned actions to build trust and correct public perception.


---

##  Limitations & Assumptions

- Salary data reflects base pay only and excludes tax, benefits, and allowances.  
- Gender classification includes a “Declined to Respond” category, which may affect the accuracy of some insights.    
- Performance ratings are treated as accurate and free from bias.  
- The analysis is based on a static dataset (a snapshot in time), and does not account for changes over time.

---

##  Suggestions for Further Analysis

- **Exit Interview Sentiment Analysis**  
  Understand reasons for employee turnover, with a focus on gender-related trends.

- **Performance Rating Bias Audit**  
  Use statistical tools to detect potential bias in how ratings are assigned.

- **Salary Growth Tracking**  
  Analyze how salaries evolve for male and female employees over time.

- **Leadership Pipeline Analysis**  
  Examine gender representation in leadership development and succession planning.

- **Predictive Equity Modeling**  
  Identify and forecast potential risks of inequity using data trends.

---

##  Conclusion

Palmoria Group is currently under justifiable scrutiny regarding gender equality, but this challenge also presents a clear opportunity for transformation. The data reveals systemic gaps in salary equity, performance recognition, and bonus distribution. However, it also highlights promising trends: strong performance among underrepresented groups and pockets of gender balance in key departments.

Female employees, in particular, show consistently high ratings, underscoring a valuable but underutilized talent pool. Addressing these disparities through structured policies, transparent salary reviews, and inclusive leadership development can pave the way for both compliance and cultural change.

By implementing the recommended actions with decisive leadership and a data-driven strategy, Palmoria has the chance to rebuild trust, foster fairness, and emerge as a model for gender equity in the manufacturing sector both within Nigeria and globally.
