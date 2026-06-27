# Calculated Fields

The following calculated fields were created in Tableau to support KPI calculations and business analysis:

## 1. Profit Margin

**Formula:**

```
SUM([Profit]) / SUM([Sales])
```

**Purpose:**
Calculates the percentage of sales retained as profit, helping evaluate overall profitability.

---

## 2. Cost

**Formula:**

```
SUM([Sales]) - SUM([Profit])
```

**Purpose:**
Estimates the total cost associated with generating sales by subtracting profit from sales.

---

## 3. Average Order Value

**Formula:**

```
SUM([Sales]) / COUNTD([Order Id])
```

**Purpose:**
Calculates the average revenue generated per unique customer order, providing insight into purchasing behavior.

---

## 4. Return Rate

**Formula:**

```
SUM([Return Flag]) / COUNT([Order Id])
```

**Purpose:**
Measures the proportion of returned orders relative to the total number of orders, helping identify return trends and product quality issues.

---

## 5. Shipping Delay Bucket

**Formula:**

```
IF [Delivery Days] <= 2 THEN "Fast (0-2 Days)"
ELSEIF [Delivery Days] <= 5 THEN "Medium (3-5 Days)"
ELSE "Delayed (6+ Days)"
END
```

**Purpose:**
Groups orders into delivery speed categories to simplify shipping performance analysis.

---

## 6. Profit Status

**Formula:**

```
IF [Profit] > 0 THEN "Profitable"
ELSE "Loss"
END
```

**Purpose:**
Classifies each transaction as profitable or loss-making, making it easier to identify products or regions that negatively impact business performance.


# Business Insights

## Insight 1: Overall Business Performance

### Observation

The business generated **$217.0M** in total sales with **$33.3M** in total profit, resulting in an overall **15.3% profit margin**.

### Data Evidence

* Total Sales: **$217.0M**
* Total Profit: **$33.3M**
* Profit Margin: **15.3%**

### Business Interpretation

The company is operating profitably with a healthy profit margin, indicating that overall revenue generation is translating into positive financial performance.

### Recommended Action

Maintain current sales performance while identifying opportunities to improve margins through pricing optimization and operational efficiency.

---

## Insight 2: Monthly Sales Trend

### Observation

Monthly sales remain relatively stable over the reporting period with normal fluctuations rather than extreme volatility.

### Data Evidence

The Monthly Sales Trend chart shows sales varying between approximately **$6.30M** and **$10.86M**, without a sustained downward trend.

### Business Interpretation

Sales demand appears consistent across the reporting period, suggesting stable customer demand and business operations.

### Recommended Action

Analyze the factors contributing to peak-performing months and replicate successful promotional or operational strategies during lower-performing periods.

---

## Insight 3: Regional Sales Performance

### Observation

The **South** region is the strongest contributor to total sales.

### Data Evidence

Regional sales are:

* South – **$64.69M**
* North – **$54.56M**
* West – **$48.91M**
* East – **$48.86M**

### Business Interpretation

The South region contributes the highest revenue, while East and West generate comparatively lower sales.

### Recommended Action

Study the sales strategy used in the South region and implement similar practices in East and West to improve overall regional performance.

---

## Insight 4: Category & Sub-Category Profitability

### Observation

Technology is the most profitable category, mainly driven by **Copiers** and **Accessories**.

### Data Evidence

Top profitable sub-categories include:

* Copiers – **$7.31M**
* Accessories – **$7.10M**

Furniture contributes moderate profit, while Office Supplies contributes comparatively smaller profits across its sub-categories.

### Business Interpretation

Technology products are the primary contributors to overall profitability and should remain a strategic focus.

### Recommended Action

Increase inventory availability and marketing investment for high-performing Technology products while improving profitability in Office Supplies and Furniture.

---

## Insight 5: Customer Segment Performance

### Observation

The **Home Office** segment generates the highest sales among all customer segments.

### Data Evidence

Customer segment sales are:

* Home Office – **$74.50M**
* Consumer – **$71.89M**
* Corporate – **$70.63M**

### Business Interpretation

Although sales are fairly balanced across segments, the Home Office segment currently contributes the highest revenue.

### Recommended Action

Continue targeted campaigns for Home Office customers while designing segment-specific marketing initiatives to increase Consumer and Corporate sales.

---

## Insight 6: Discount Impact on Profitability

### Observation

Higher discount percentages are associated with an increase in low-profit and loss-making orders.

### Data Evidence

The Discount vs Profit Relationship chart shows that most high-profit orders occur at lower discount levels, while negative-profit transactions become more frequent as discount percentages increase.

### Business Interpretation

Heavy discounting reduces profitability and increases the risk of losses.

### Recommended Action

Review discount policies and establish approval limits for high discount levels to protect overall profit margins.

---

## Insight 7: Business Opportunity

### Observation

Technology products consistently outperform other categories in terms of profitability.

### Data Evidence

Multiple Technology sub-categories dominate the profitability chart, with Copiers and Accessories generating the highest profits.

### Business Interpretation

Technology represents the company's strongest opportunity for future revenue and profit growth.

### Recommended Action

Prioritize Technology products through additional promotions, inventory investment, and cross-selling opportunities.

---

## Insight 8: Dashboard Limitation and Future Analysis

### Observation

The current executive dashboard focuses primarily on sales and profitability performance.

### Data Evidence

The dashboard includes KPI cards, Monthly Sales Trend, Regional Sales Performance, Category & Sub-Category Profitability, Customer Segment Sales Performance, and Discount vs Profit Relationship.

### Business Interpretation

Important operational metrics such as shipping performance and product returns are not currently included, limiting visibility into logistics efficiency and customer satisfaction.

### Recommended Action

Expand future versions of the dashboard by including Shipping Performance and Return Analysis to support more comprehensive business decision-making.
