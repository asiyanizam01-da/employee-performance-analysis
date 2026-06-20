# Employee Performance Analytics — Excel Project

End-to-end HR analytics project built entirely in Microsoft Excel — covering data validation, KPI development, Pivot Table analysis, and dashboard design to turn raw employee performance data into actionable workforce insights.

## Project Overview

This project analyzes employee performance data to evaluate workforce productivity, identify high and low performers, and uncover trends across departments, roles, gender, and age groups.

It demonstrates a full analytics workflow — data validation, feature engineering, exploratory analysis, KPI development, and dashboard creation — using only native Excel tools.

## Tools Used

- Microsoft Excel
- Pivot Tables
- Excel Formulas (`IFS`, `COUNTIF`, `AVERAGE`, `FILTER`, `SORT`)
- Data Validation Techniques
- Dashboard Visualization

## Dataset

> **Note:** This dataset is synthetically generated using AI. It simulates realistic HR performance patterns — including department-specific KPIs, seasonal trends, and natural performance variance — for analytics practice and portfolio purposes. It does not represent real employees, real companies, or real confidential HR data.

The project uses two related tables:

**Employee Data** — demographic and organizational information
| Column | Description |
|---|---|
| `employee_id` | Unique employee identifier |
| `name` | Full name |
| `role` | Job title |
| `department` | Department name |
| `age` | Employee age |
| `gender` | Employee gender |
| `join_date` | Date of hire |

**Employee Performance** — monthly performance records
| Column | Description |
|---|---|
| `employee_id` | Foreign key to Employee Data |
| `month` | Reporting month (YYYY-MM) |
| `target` | Monthly performance target |
| `achieved` | Monthly actual result |

**Dataset Summary**
| Metric | Value |
|---|---|
| Employees | 100 |
| Performance records | 1,129 |
| Departments | 7 |
| Time period | Jan – Dec 2025 (12 months) |

## Project Workflow

### 1. Data Validation
Performed data quality checks including:
- Duplicate employee ID checks
- Missing value checks
- Age validation
- Join date validation
- Target validation
- Achievement validation
- Employee-month uniqueness validation

All validation checks passed successfully.

### 2. Feature Engineering
Created additional analytical fields:
- Performance Percentage = Achieved ÷ Target
- Performance Status (Excellent, Good, Average, Poor)
- Employee Rank
- Age Group Classification

### 3. Exploratory Data Analysis
Analysis was conducted to answer the following business questions:
- Which employees achieve the highest performance?
- Which departments perform the best?
- Which departments underperform?
- How does performance change over time?
- Which roles perform best?
- Does performance vary by gender?
- Does performance vary by age group?
- Which employees require performance improvement?

## Key Insights

- Average employee performance was **95.67%**
- **Engineering** was the highest-performing department (**105.04%**)
- **Customer Support** was the lowest-performing department (**84.09%**)
- Employee performance remained relatively stable throughout the year
- Performance reached its lowest point in **August** (91.09%)
- Performance peaked in **November** (100.88%)
- Gender-based performance differences were minimal
- Senior employees recorded the highest average performance
- Most employees were classified within the **Average** performance category

## Dashboard

A one-page Excel dashboard was created to visualize key performance metrics and trends.

**KPI Cards**
- Total Employees
- Average Performance
- Best Performing Department
- Excellent Employees
- Employees Requiring Improvement

**Visualizations**
- Monthly Performance Trend
- Employee Performance Distribution
- Department Performance Comparison
- Top 10 Performers

## Skills Demonstrated

- Data Cleaning & Validation
- KPI Development
- Workforce Performance Analysis
- Pivot Table Reporting
- Data Visualization
- Dashboard Design
- Business Insight Generation

## Project Structure

```text
employee-performance-excel-analytics/
├── data/
│   ├── employee_data.csv
│   └── employee_performance.csv
├── dashboard/
│   └── employee_performance_dashboard.xlsx
├── screenshots/
│   └── dashboard.png
└── README.md
```

## Getting Started

1. Clone or download this repository.
2. Open `dashboard/employee_performance_dashboard.xlsx` in Excel.
3. If prompted, enable content/macros and allow formulas to recalculate.
4. Explore the Pivot Tables and Dashboard sheet, or refresh them against the raw CSVs in `data/` to verify the analysis.

## Conclusion

This project demonstrates how Excel can be used to perform end-to-end HR analytics by combining data validation, performance measurement, trend analysis, and dashboard reporting. The resulting insights provide a clear view of workforce productivity and departmental performance while supporting data-driven decision-making.
