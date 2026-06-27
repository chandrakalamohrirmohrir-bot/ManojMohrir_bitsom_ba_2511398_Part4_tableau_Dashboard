# Task 1: Data Connection and Inspection

## Data Inspection Summary

The dataset was successfully connected to Tableau Public using the Microsoft Excel connector. The workbook contains two sheets: **dashboard_sales_data**, which was used for analysis, and **data_dictionary**, which was used as a reference to understand the fields. The primary data sheet contains **4,200 records** and **20 fields**.

The data types were reviewed to ensure they were correctly recognized by Tableau before creating visualizations.

### Date Fields

* Order Date
* Ship Date

Both fields were correctly identified as date fields and will be used for trend analysis and delivery performance calculations.

### Geographic Fields

* State
* City
* Region

These fields support geographic analysis and regional performance comparisons. Tableau recognizes State and City as geographic fields for mapping.

### Categorical Fields

* Category
* Sub Category
* Customer Segment
* Ship Mode
* Campaign Channel
* Product Name
* Customer ID
* Order ID

These fields represent descriptive business information and will be used for grouping, filtering, and comparison across different business dimensions.

### Numerical Measures

* Sales
* Profit
* Quantity
* Discount
* Customer Rating
* Delivery Days

These numeric fields will be used to calculate KPIs, perform profitability analysis, measure operational performance, and create calculated fields such as Profit Margin, Cost, Average Order Value, and Return Rate.

### Binary / Flag Fields

* Returned

The Returned field acts as a binary indicator showing whether an order was returned. It will be used to calculate return rates and identify return patterns across categories, regions, and customer segments.

## Assumptions

* The dataset is assumed to be complete and suitable for dashboard development.
* Sales and Profit values are assumed to be recorded in the same currency.
* Delivery Days represents the difference between Ship Date and Order Date.
* Each Order ID represents a unique customer order unless otherwise specified.
* Missing or invalid values, if any, are assumed to have been addressed before the dashboard development phase.
* The Returned field contains consistent values that accurately indicate whether an order was returned.


# Retail Executive Performance Dashboard

## Business Problem Summary

The objective of this project is to design an executive-level Tableau dashboard that helps business leaders monitor overall sales performance, profitability, regional performance, customer segments, product profitability, and the impact of discounting. The dashboard provides an interactive overview that supports data-driven business decisions.

---

# Dataset Description

The dashboard is built using a retail sales dataset containing transactional order information.

The dataset includes information such as:

* Order Date
* Region
* Category
* Sub-Category
* Customer Segment
* Sales
* Profit
* Discount
* Quantity
* Ship Mode

The dataset was cleaned before visualization, and calculated fields were created to derive additional business metrics.

---

# Tableau Workbook Description

The Tableau workbook contains an executive dashboard designed for leadership reporting.

The dashboard combines KPI cards with multiple analytical visualizations to present sales, profitability, regional contribution, customer behavior, product profitability, and discount analysis in a single interactive view.

---

# Calculated Fields Created

The following calculated fields were created:

* Profit Margin
* Profit Status
* Return Rate
* Shipping Delay Bucket
* Delivery Days
* Average Order Value

These calculated fields were used to improve business analysis and support dashboard visualizations.

---

# Dashboard Components

The executive dashboard contains:

## KPI Cards

* Total Sales
* Total Profit
* Profit Margin

## Visualizations

* Monthly Sales Trend
* Regional Sales Performance
* Category & Sub-Category Profitability
* Customer Segment Sales Performance
* Discount vs Profit Relationship

---

# Filters and Dashboard Interactions

The dashboard includes interactive filters for:

* Region
* Category
* Customer Segment

Dashboard action filters allow users to click on a region, category, or customer segment and automatically filter the remaining dashboard views.

---

# Key Business Insights

* The business generated **$217.0M** in total sales and **$33.3M** in total profit.
* Overall Profit Margin is **15.3%**.
* The South region contributes the highest sales.
* Technology is the most profitable category, driven primarily by Copiers and Accessories.
* Home Office is the highest-performing customer segment by sales.
* Higher discount levels are associated with lower profitability and more loss-making transactions.

---

# Dashboard Story Summary

The dashboard shows that the business is financially healthy, supported by strong sales and positive profitability.

Regional analysis identifies the South as the strongest market, while Technology products contribute the highest profits. Customer sales are relatively balanced across segments, with Home Office generating the highest revenue. The dashboard also highlights the relationship between discounting and profitability, demonstrating that excessive discounts can negatively affect profits.

Overall, the dashboard helps executives identify strengths, monitor performance, and recognize opportunities for future improvement.

---

# Assumptions and Limitations

## Assumptions

* The dataset accurately represents completed retail transactions.
* All calculated fields are based on cleaned data.
* Profit Margin is calculated using Profit ÷ Sales.

## Limitations

* Shipping performance metrics are not included in the final dashboard.
* Product return analysis is not included in the final dashboard.
* Customer satisfaction metrics are unavailable.
* The dashboard focuses on descriptive analysis and does not include forecasting.

---

# Screenshots Included

The repository contains the following screenshots:

* full_dashboard.png
* sales_trend_view.png
* regional_performance_view.png
* category_profitability_view.png
* filter_interaction_view.png

---

# Repository Structure

```
project/
│
├── data/
│   └── dashboard_sales_data.xlsx
│
├── outputs/
│   ├── business_insights.md
│   ├── dashboard_story.md
│   ├── chart_selection_justification.md
│   ├── full_dashboard.png
│   ├── sales_trend_view.png
│   ├── regional_performance_view.png
│   ├── category_profitability_view.png
│   └── filter_interaction_view.png
│
├── tableau/
│   └── Executive_Dashboard.twb
│
└── README.md
```

## Conclusion

This executive dashboard provides a clear and interactive summary of business performance by combining financial KPIs with visual analysis of sales trends, regional performance, customer segments, category profitability, and discount impact. It enables leadership to quickly identify business strengths, potential risks, and areas requiring strategic action.
