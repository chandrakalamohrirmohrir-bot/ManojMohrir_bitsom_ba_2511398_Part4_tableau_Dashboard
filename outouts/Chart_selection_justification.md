# Chart Selection Justification

# Executive Sales Dashboard – Chart Selection Justification

## Dashboard Overview

The Executive Sales Dashboard was designed to provide senior management with a concise overview of business performance. It combines key performance indicators with visual analytics to help executives monitor sales, profitability, regional performance, customer segments, product profitability, and the impact of discounting on profit.

---

# Visualization Design Principles

## 1. KPI Cards

### Charts Used

* Total Sales
* Total Profit
* Profit Margin

### Purpose

The KPI cards present the most important business metrics at the top of the dashboard, allowing executives to understand overall business performance immediately.

### Justification

KPI cards provide a quick performance summary before users explore detailed visualizations.

---

## 2. Monthly Sales Trend

### Chart Type

Line Chart

### Business Question

How have monthly sales changed over time?

### Justification

A line chart is the most appropriate visualization for time-series data because it clearly displays upward and downward sales movements across months while making trends easy to identify.

---

## 3. Regional Sales Performance

### Chart Type

Horizontal Bar Chart

### Business Question

Which regions generate the highest sales?

### Justification

A horizontal bar chart enables easy comparison between regions. Sorting the regions by sales allows executives to immediately identify the strongest and weakest performing markets.

---

## 4. Category & Sub-Category Profitability

### Chart Type

Horizontal Bar Chart

### Business Question

Which categories and sub-categories contribute the highest profit?

### Justification

The horizontal bar chart allows direct comparison of profits across categories and sub-categories while keeping long category names readable. The chart highlights the most profitable product groups and supports product portfolio decisions.

---

## 5. Customer Segment Sales Performance

### Chart Type

Vertical Bar Chart

### Business Question

Which customer segment contributes the highest sales?

### Justification

A vertical bar chart is ideal for comparing sales across discrete customer segments. It provides a clear visual comparison between Home Office, Consumer, and Corporate customers.

---

## 6. Discount vs Profit Relationship

### Chart Type

Scatter Plot

### Business Question

How does discount affect profitability?

### Justification

A scatter plot is the best visualization for studying the relationship between two continuous variables. It allows executives to observe how increasing discounts influence profit while identifying profitable and loss-making transactions.

---

# Dashboard Design Principles

## Correct Chart Selection

Each visualization was selected according to the business question being answered.

* KPI Cards for summary metrics
* Line Chart for sales trends over time
* Horizontal Bar Charts for regional and category comparisons
* Vertical Bar Chart for customer segment comparison
* Scatter Plot for analysing the relationship between discount and profit

---

## Clear Hierarchy

The dashboard follows a logical executive reporting structure.

1. Business KPIs
2. Monthly Sales Trend
3. Regional Performance
4. Customer Segment Performance
5. Product Profitability
6. Discount Impact Analysis

This arrangement enables users to move from high-level business performance to detailed operational insights.

---

## Minimal Clutter

The dashboard contains only business-relevant visualizations.

Unnecessary gridlines, labels, and decorative elements have been minimized to improve readability while keeping the dashboard clean and professional.

---

## Consistent Color Usage

A consistent blue color palette is used across KPI cards, regional performance, customer segment performance, and sales trend visualizations.

The profitability chart uses different colors to distinguish product categories, while the scatter plot uses green and red to differentiate profitable and loss-making transactions.

---

## Proper Labels

Every visualization includes:

* Clear chart titles
* Appropriate axis labels
* Data labels where useful
* Business-friendly number formatting using millions (M)

---

## Readable Titles

All chart titles clearly describe the business question being answered, allowing users to interpret each visualization without additional explanation.

---

## Appropriate Sorting

Regional performance is displayed in descending sales order, while category profitability highlights the highest-profit categories first, enabling faster identification of key business contributors.

---

## Useful Filters and Dashboard Actions

Interactive dashboard filters allow users to explore business performance by Region, Category, and Customer Segment.

Dashboard actions enable users to click visualizations and dynamically filter the remaining charts, supporting interactive analysis.

---

## Avoidance of Misleading Scales

Bar charts begin from zero where appropriate, ensuring accurate visual comparisons.

The line chart uses a consistent time scale to display monthly sales without exaggerating fluctuations.

---

## Business Interpretation

The dashboard focuses on business decision-making rather than simply displaying numbers.

Executives can quickly understand:

* Overall business performance
* Monthly sales movement
* Regional contribution
* Customer segment performance
* Product profitability
* The impact of discounting on profit

This enables faster, data-driven strategic decisions.


# Chart Selection Justification

## 1. KPI Cards (Total Sales, Total Profit, Profit Margin)

### Question the chart answers

What is the overall business performance at a glance?

### Why this chart type is appropriate

KPI cards allow executives to immediately understand the company's key financial metrics without interpreting detailed charts. They provide a quick summary of business performance.

### Visual encodings used

* Large text emphasizes important business metrics.
* Simple formatting keeps attention on the values.
* Positioned at the top of the dashboard to establish context before viewing detailed charts.

### Design principle applied

Clear visual hierarchy. The most important business metrics are displayed first for quick decision-making.

### Mistake avoided

Avoided using charts for single values, which would waste dashboard space and reduce readability.

---

## 2. Monthly Sales Trend (Line Chart)

### Question the chart answers

How has monthly sales performance changed over time?

### Why this chart type is appropriate

A line chart is the best choice for displaying trends across time because it clearly shows increases, decreases, and seasonal fluctuations.

### Visual encodings used

* X-axis represents Month of Order Date.
* Y-axis represents Sales.
* Data labels highlight important values.
* A single color keeps the trend easy to follow.

### Design principle applied

Consistency and simplicity were maintained so users can quickly recognize long-term sales patterns.

### Mistake avoided

Avoided using bar charts for time-series data, which would make trend identification more difficult.

---

## 3. Regional Sales Performance (Horizontal Bar Chart)

### Question the chart answers

Which regions contribute the most sales?

### Why this chart type is appropriate

Horizontal bar charts make it easy to compare values across categories and accommodate longer region names.

### Visual encodings used

* Bar length represents total sales.
* Consistent blue color emphasizes comparison rather than highlighting individual regions.
* Value labels display exact sales figures.
* Regions are sorted from highest to lowest sales.

### Design principle applied

Sorted ordering improves readability and allows executives to identify top-performing regions quickly.

### Mistake avoided

Avoided pie charts because they make comparing multiple regional values less accurate.

---

## 4. Category & Sub-Category Profitability (Horizontal Bar Chart)

### Question the chart answers

Which categories and sub-categories generate the highest profits?

### Why this chart type is appropriate

A horizontal bar chart clearly compares profitability across multiple categories and sub-categories while making ranking easy to understand.

### Visual encodings used

* Bar length represents profit.
* Different colors distinguish the main product categories.
* Value labels display exact profit values.
* Categories and sub-categories are grouped logically.

### Design principle applied

Grouping related products improves business interpretation and helps identify the strongest profit contributors.

### Mistake avoided

Avoided stacked charts that could make comparing individual sub-category profits more difficult.

---

## 5. Customer Segment Sales Performance (Vertical Bar Chart)

### Question the chart answers

How does sales performance differ across customer segments?

### Why this chart type is appropriate

A vertical bar chart is effective for comparing sales among a small number of customer segments.

### Visual encodings used

* Bar height represents sales.
* Different shades of blue distinguish customer segments.
* Value labels provide exact sales amounts.

### Design principle applied

Minimal clutter and consistent formatting improve readability and support quick comparisons.

### Mistake avoided

Avoided unnecessary color variation that could distract from the actual comparison.

---

## 6. Discount vs Profit Relationship (Scatter Plot)

### Question the chart answers

How does discount level influence profitability?

### Why this chart type is appropriate

A scatter plot is the most appropriate chart for identifying relationships between two continuous variables and revealing patterns, clusters, and outliers.

### Visual encodings used

* X-axis represents Discount.
* Y-axis represents Profit.
* Colors distinguish profitable and loss-making orders.
* Individual points represent orders.

### Design principle applied

Color is used meaningfully to separate profitable transactions from loss-making transactions, making patterns easier to identify.

### Mistake avoided

Avoided line or bar charts because they cannot effectively display the relationship between discount and profit for individual orders.

---

# Overall Dashboard Design

The dashboard follows a clear executive layout. KPI cards are placed at the top to summarize business performance, followed by trend analysis, regional comparison, profitability analysis, customer segment performance, and discount impact. Consistent colors, readable titles, appropriate chart types, and minimal visual clutter make the dashboard easy to interpret while supporting effective business decision-making.
