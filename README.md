# 📊 Task 4 – Data Storytelling & Statistical Validation

## 📌 Project Overview
This project was completed as part of my Data Analytics Internship at ApexPlanet Software Pvt. Ltd.
The objective of Task 4 was to synthesize all previous analysis into a compelling business narrative and use basic statistical methods to add rigor and validate key findings.
For this project, I took the insights generated from Parts 1-3, formulated a testable business hypothesis regarding profit margins, performed statistical validation, and developed a professional presentation to communicate actionable recommendations to stakeholders.

## 🎯 Objective
The main objectives of this project were:
* Craft a cohesive data story from Parts 1-3 for a business audience.
* Formulate a testable business hypothesis based on EDA findings.
* Perform an appropriate statistical test to validate the findings.
* Develop a professional presentation deck focusing on business impact.[cite: 1]
* Generate actionable root-cause business recommendations.[cite: 1]

## 🗂️ Dataset
The project synthesizes the datasets cleaned and explored in previous tasks:
* Task 1 & 2: Retail sales data consisting of 1,005 raw records (995 retained after cleaning).[cite: 1]
* Task 3: Superstore dataset containing 5,111 orders across 4 years.[cite: 1]

**Data Workflow**
Raw Data → Data Cleaning (Task 1) → EDA (Task 2) → Deep-Dive (Task 3) → Statistical Validation & Storytelling (Task 4)

## 🧹 Previous Tasks Summary
The foundation for this data story was built upon three previous phases:
* **Task 1 (Clean):** 1,005 raw sales records inspected; missing values, duplicates, and bad dates fixed to retain 995 valid records.[cite: 1]
* **Task 2 (Explore):** SQL cleaning and Excel BI dashboard built to answer 7 core business questions, revealing regional performance gaps.[cite: 1]
* **Task 3 (Deep-Dive):** Python and Tableau used to define KPIs, identifying a major red flag: Furniture generated $754.7K in sales but only $19.7K in profit (a 2.6% margin vs 17%+ for other categories).[cite: 1]

## 🔎 Hypothesis Testing & Statistical Validation
To ensure the observed margin gap wasn't a coincidence, a statistical test was conducted.[cite: 1]
Areas analyzed:
* **H₀ — Null Hypothesis:** There is no significant difference in profit margin between the Furniture category and other product categories.[cite: 1]
* **H₁ — Alternative Hypothesis:** Furniture's profit margin is significantly lower than that of other product categories.[cite: 1]
* **Test Selected:** Independent Samples T-Test (Welch's correction) with a significance level of α = 0.05.[cite: 1]

## 📊 Statistical Results
The hypothesis testing yielded the following results:

| Metric | Value |
| :--- | :--- |
| **t-statistic** | -11.03[cite: 1] |
| **p-value** | 5.8 × 10⁻²⁸ (p < 0.001)[cite: 1] |
| **Mean difference** | -10.15 points[cite: 1] |
| **95% Confidence interval** | [-11.95, -8.34][cite: 1] |

**Decision:** Reject H₀ — the gap is statistically significant, not chance.[cite: 1]

## 📈 Final Presentation Deck
A professional presentation was created to communicate these findings.
**Deck Components**
* Executive Summary
* Task 1-3 Phase Breakdowns
* The Red Flag (Profitability Gap)
* Hypothesis Formulation & Testing
* Root-Cause Analysis (Sub-category drill-down)
* Business Recommendations

## 💡 Key Business Insights & Recommendations
The root-cause analysis revealed that not all furniture is the problem; Chairs and Furnishings are profitable, but Tables and Bookcases are net loss-making due to high discounts.[cite: 1]
Actionable recommendations include:
* **Cap discounts on Tables and Bookcases:** Cap at 15% and monitor margin recovery, as they currently sell at 22–26% average discount.[cite: 1]
* **Renegotiate Tables supplier cost:** A discount cap alone may not fix a -$17.8K loss on Tables; base costs need review.[cite: 1]
* **Redirect growth spend:** Shift focus to Technology & Office Supplies, which carry proven 17%+ margins.[cite: 1]
* **Make this a quarterly check:** Re-run the same t-test each quarter to catch margin erosion early.[cite: 1]

## 🛠️ Tools & Technologies
* 🐍 Python (SciPy/Statsmodels for Hypothesis Testing)
* 📊 Tableau & Excel (Reference Visualizations)
* 📑 PowerPoint / Google Slides (Presentation Design)
* 🐙 GitHub
* 📈 Statistical Analysis
* 🗣️ Data Storytelling

## 📁 Project Structure
```text
Task-4-Data-Storytelling-Statistical-Validation/
│
├── README.md
├── presentation/
│   └── Task_4_Final_Presentation.pptx
│   └── Task_4_Final_Presentation.pdf
├── statistics/
│   └── hypothesis_testing_summary.md
└── insights/
    └── business_recommendations.md