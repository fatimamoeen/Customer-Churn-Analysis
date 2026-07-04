<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3B4A3F,100:52B788&height=200&section=header&text=Telecom%20Customer%20Churn%20EDA&fontSize=38&fontColor=FFFFFF&animation=fadeIn&fontAlignY=38&desc=Exploratory%20Data%20Analysis%20%7C%20Portfolio%20Project&descAlignY=58&descSize=16" width="100%"/>

![Python](https://img.shields.io/badge/Python-3B4A3F?style=for-the-badge&logo=python&logoColor=52B788)
![Pandas](https://img.shields.io/badge/Pandas-3B4A3F?style=for-the-badge&logo=pandas&logoColor=52B788)
![Jupyter](https://img.shields.io/badge/Jupyter-3B4A3F?style=for-the-badge&logo=jupyter&logoColor=52B788)
![Tableau](https://img.shields.io/badge/Tableau-3B4A3F?style=for-the-badge&logo=tableau&logoColor=52B788)
![Status](https://img.shields.io/badge/Status-Complete-52B788?style=for-the-badge)

</div>

## Table of Contents

- [Project Overview](#project-overview)
- [Business Objective](#business-objective)
- [Dataset](#dataset)
- [Tools & Tech Stack](#tools--tech-stack)
- [Data Cleaning & Transformation](#data-cleaning--transformation)
- [Key Insights](#key-insights)
- [Highest-Impact Churn Drivers](#highest-impact-churn-drivers)
- [Financial Impact](#financial-impact)
- [Business Recommendations](#business-recommendations)
- [Interactive Dashboard](#interactive-dashboard)
- [Repository Structure](#repository-structure)
- [What I Learned](#what-i-learned)
- [Author](#author)

## Project Overview

| | |
|---|---|
| **Project** | Telecom Customer Churn — Exploratory Data Analysis |
| **Type** | Personal portfolio project |
| **Focus area** | Business analytics / data-driven decision making |
| **Dataset size** | 7,043 customer records · 20 features |
| **Overall churn rate** | 26.54% |
| **Deliverables** | Python EDA notebook · Business report · Tableau interactive dashboard |

## Business Objective

Telecom companies lose recurring revenue every time a customer churns, and replacing a lost customer costs more than retaining one. I built this project to practice framing a raw dataset as a real business problem — not just running charts, but turning them into decisions. The analysis answers four questions:

1. What is the overall churn rate, and which segments churn the most?
2. Which service offerings, contract types, and payment methods correlate with higher churn?
3. What is the financial exposure created by churn?
4. What retention actions should be prioritised, and in what order?

## Dataset

- **Source:** Telco Customer Churn dataset (Kaggle / IBM sample dataset)
- **Size:** 7,043 rows × 20 columns (demographic, account, and service-usage features, plus the churn label)
- **Features include:** gender, senior citizen status, tenure, contract type, internet service, payment method, monthly charges, tech support, online security, and more

## Tools & Tech Stack

| Category | Tools |
|---|---|
| Data analysis | Python — Pandas, NumPy |
| Visualisation | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |
| Reporting | HTML/CSS (self-built business report) |
| Dashboard | Tableau Public (interactive) |

## Data Cleaning & Transformation

- Handled `FutureWarning`s from pandas groupby/aggregation syntax
- Resolved duplicate column errors during merge/concat operations
- Converted `TotalCharges` to numeric, handled blank strings from missing values
- Bucketed `tenure` into readable bands (0–12, 13–24, 25–48, 49+ months) for cleaner visualisation

## Key Insights

- **26.54%** of customers have churned overall — roughly 1 in 4
- **Month-to-month contracts** churn at 42.7% vs just 2.8% for two-year contracts
- **Electronic check** users churn at 45.3%, the highest of any payment method
- **Fiber optic** users churn at 41.9%, nearly matching contract-type churn
- Customers **without tech support or online security** churn at ~42% vs ~14–15% with those add-ons — a 3x difference
- **Senior citizens** churn at nearly double the rate of non-seniors
- **Gender has no meaningful effect** on churn
- Churn is heavily concentrated in the **first 0–12 months of tenure**
- Churned customers pay **more per month (~$74) than retained customers (~$61)** — the customers most likely to leave are also above-average revenue generators

## Highest-Impact Churn Drivers

| Attribute | Highest-risk group | Approx. churn rate |
|---|---|---|
| Payment method | Electronic check | 45.3% |
| Contract type | Month-to-month | 42.7% |
| Internet service | Fiber optic | 41.9% |
| Online security | No online security | 41.8% |
| Tech support | No tech support | 41.6% |

## Financial Impact

- Estimated monthly revenue exposure from churn: **~$138K**
- Annualised exposure: **~$1.66M**
- Churned customers carry higher average monthly charges than retained customers, meaning churn removes above-average revenue, not just headcount

## Business Recommendations

**Immediate**
1. Launch a contract-conversion incentive for month-to-month customers (critical priority)
2. Build a 90-day onboarding retention track for early-tenure customers
3. Target senior citizen customers with dedicated support

**Medium term**

4. Bundle online security & tech support into mid-tier plans
5. Investigate fiber optic service dissatisfaction
6. Shift electronic check users toward automatic payment methods

**Long term**

7. Build a churn-propensity scoring model (logistic regression / Random Forest)
8. Establish a quarterly churn-driver review process

## Interactive Dashboard

View the live, filterable Tableau dashboard here: **[Tableau Public link — add here]**

The dashboard lets you filter by gender and senior citizen status across all seven churn dimensions covered in this analysis.

## Repository Structure

```
telecom-churn-eda/
│
├── README.md
├── requirements.txt
├── Customer_Churn_EDA.ipynb          # Full Python EDA notebook
├── Customer_Churn_Report       # business report (single-file)
├── data/
│   └── telco_customer_churn.csv
├── assets/
│   ├── churn_distribution.png
│   ├── churn_by_gender_senior.png
│   ├── churn_by_tenure.png
│   ├── churn_by_service_drivers_1.png
│   ├── churn_by_service_drivers_2.png
│   ├── monthly_charges_impact.png
│   └── dashboard_snapshot.png
└── dashboard/
    └── tableau_dashboard_link.txt
```


## What I Learned

- How to move from raw EDA to a structured business narrative — quantifying risk, not just describing patterns
- Practical debugging: pandas `FutureWarning`s, duplicate-column errors, and `wkhtmltopdf` CSS quirks while building the HTML report
- How to design a Tableau dashboard with a deliberate color system instead of default palettes
- The difference between a chart that's technically correct and one that actually drives a decision

## Author

**Fatima Moeen**
BSc (Hons) Computer Science, Jamia Millia Islamia
Building toward a Data Analyst / FinTech career path

## Dashboard
<img width="1472" height="882" alt="image" src="https://github.com/user-attachments/assets/be6e59df-449d-4def-8d99-121ce7f4cbaf" />

