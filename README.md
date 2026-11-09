# Customer Churn Analysis and Retention Strategy

**A Data-Driven Business Intelligence Project**

## Project Overview

Customer churn occurs when customers discontinue a service or subscription. Understanding customer churn helps businesses identify retention challenges and develop strategies to improve customer loyalty.

This project analyses customer data using Python, exploratory data analysis (EDA), and statistical hypothesis testing to identify patterns associated with customer churn and recommend data-driven retention strategies.

## Business Problem

Businesses need to understand which customer characteristics are associated with churn so that they can develop appropriate retention strategies.

This project investigates the following questions:

- What percentage of customers have churned?
- How does customer tenure relate to churn?
- Do monthly charges differ between retained and churned customers?
- Is contract type associated with customer churn?
- Do churn rates vary across payment methods?
- What retention strategies can be recommended based on the findings?

## Project Objectives

1. Measure customer churn and retention rates.
2. Inspect and prepare the customer dataset.
3. Perform exploratory data analysis.
4. Identify patterns across tenure, monthly charges, contract types, and payment methods.
5. Conduct statistical hypothesis testing.
6. Develop actionable customer-retention recommendations.

## Dataset Description

The dataset contains **500 customer records and 9 attributes**.

| Attribute | Description |
|---|---|
| CustomerID | Unique customer identifier |
| Tenure | Customer tenure in months |
| MonthlyCharges | Monthly amount charged |
| TotalCharges | Total amount charged |
| Contract | Customer contract type |
| PaymentMethod | Customer payment method |
| PaperlessBilling | Paperless billing status |
| SeniorCitizen | Senior citizen indicator |
| Churn | Customer churn status |

**Churn coding:**
- `0` – Customer retained / stayed
- `1` – Customer churned / left

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## Project Structure

```text
customer-churn-business-analysis/
│
├── data/
│   ├── raw_data.csv
│   └── cleaned_data.csv
│
├── notebooks/
│   ├── 1_data_cleaning.ipynb
│   ├── 2_eda.ipynb
│   └── 3_analysis.ipynb
│
├── reports/
│   ├── executive_summary.pdf
│   └── technical_report.pdf
│
├── presentations/
│   └── business_presentation.pptx
|____ requirements.txt
|____ capstone_analysis.ipynb
│
└── README.md
```

## Project Workflow

### 1. Data Cleaning

- Inspected dataset dimensions and data types.
- Checked missing values and duplicate records.
- Verified unique customer identifiers.
- Reviewed categorical values and numerical ranges.
- Exported the validated dataset as `cleaned_data.csv`.

### 2. Exploratory Data Analysis

Performed analysis of:

- Customer churn distribution.
- Customer tenure.
- Contract type.
- Monthly charges.
- Payment methods.
- Paperless billing.
- Correlation between numerical variables and churn.

### 3. Statistical Analysis

Three statistical tests were performed using a significance level of 0.05.

| Analysis | Statistical Test | P-value | Decision |
|---|---|---:|---|
| Tenure vs Churn | Welch's t-test | 8.98 × 10⁻¹³⁰ | Reject H₀ |
| Monthly Charges vs Churn | Welch's t-test | 0.0101 | Reject H₀ |
| Contract Type vs Churn | Chi-square test | 9.59 × 10⁻⁷ | Reject H₀ |

## Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Customers | 500 |
| Retained Customers | 447 |
| Churned Customers | 53 |
| Retention Rate | 89.4% |
| Churn Rate | 10.6% |
| Average Tenure | 36.53 months |

## Key Findings

1. **Customer Tenure:** Retained customers had an average tenure of 40.15 months, while churned customers had an average tenure of 6 months.

2. **Monthly Charges:** Churned customers had higher average monthly charges (129.77) than retained customers (111.72).

3. **Contract Type:** Month-to-month contracts had the highest observed churn rate at 20.59%.

4. **Payment Method:** Credit Card customers had the highest observed churn rate among payment methods at 13.48%.

5. **Correlation:** Tenure had a moderate negative correlation with churn (−0.51).

These findings represent statistical relationships in the analysed dataset and do not establish causation.

## Business Recommendations

- Strengthen customer onboarding and early engagement.
- Review pricing strategies and communicate service value.
- Explore suitable incentives for long-term contracts.
- Investigate differences in customer payment patterns.
- Monitor churn rate, retention rate, and customer tenure regularly.

## How to Run the Project

### Prerequisites

Install Python and Jupyter Notebook.

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual repository URL.

### Step 2: Navigate to the project folder

```bash
cd customer-churn-business-analysis
```

### Step 3: Install required libraries

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the notebooks in order

1. `1_data_cleaning.ipynb`
2. `2_eda.ipynb`
3. `3_analysis.ipynb`

Run the notebooks from the `notebooks` directory so their relative data paths resolve correctly.

## Project Deliverables

- Cleaned customer dataset.
- Three Jupyter notebooks covering data cleaning, EDA, and statistical analysis.
- One-page Executive Summary PDF.
- Technical Report PDF.
- Business Presentation PowerPoint.

## Limitations and Future Scope

### Limitations

- The analysis uses 500 customer records.
- The dataset contains a limited number of customer attributes.
- Statistical relationships do not establish causation.
- No predictive machine learning model was developed.

### Future Scope

- Develop machine learning models to predict customer churn.
- Perform deeper customer segmentation.
- Build an interactive business intelligence dashboard.
- Evaluate retention strategies through controlled experiments.
- Automate customer churn monitoring.

## Conclusion

This project demonstrates how Python-based data analytics and statistical methods can be used to understand customer churn patterns and support business decision-making.

The analysis identified significant relationships between churn and customer tenure, monthly charges, and contract type. The findings provide a foundation for developing targeted customer-retention strategies.

---

**Project Category:** Data Analytics | Business Intelligence

**Tools:** Python | Pandas | NumPy | Matplotlib | Seaborn | SciPy | Jupyter Notebook
