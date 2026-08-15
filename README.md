# Superstore Sales & Profit Analysis

An end-to-end data analytics project using **PostgreSQL, SQL, Power BI, and DAX** to analyze sales performance, profitability, discount impact, and regional performance.

## Project Overview

This project analyzes the Superstore dataset to identify business performance trends and understand the factors associated with profitability.

The analysis focuses on:

- Sales and profit performance
- Category and sub-category profitability
- Regional performance
- Discount and profit relationship
- Loss-making sub-categories
- High-discount risk areas
- Discount optimization through What-If analysis
- Data-driven business recommendations

## Business Questions

- Which sub-categories are generating losses?
- Which regions are performing best and worst?
- How are discount levels associated with profitability?
- At what discount levels does profitability become negative?
- Which areas require better pricing or discount control?
- How can What-If analysis support discount decisions?

## Tools & Technologies

- **PostgreSQL** — SQL-based data analysis
- **SQL** — Data exploration and business analysis
- **Power BI** — Interactive dashboard and visualization
- **DAX** — Measures and What-If analysis
- **GitHub** — Project documentation and version control

## Key Insights

### 1. Tables is the biggest loss-making sub-category

- Total sales: **$206.97K**
- Total profit: **-$17.73K**
- Average discount: **26.13%**
- Tables generated the largest loss among the analyzed sub-categories.

### 2. Higher discounts are associated with lower profitability

- **0% discount** generated approximately **$320.99K** in total profit.
- **30% discount** generated approximately **-$10.37K** in total profit.
- **70% discount** generated approximately **-$40.08K** in total profit.
- **80% discount** generated approximately **-$30.54K** in total profit.

This indicates that excessive discounting is strongly associated with negative profitability in the dataset.

### 3. Tables and Bookcases become unprofitable at higher discounts

**Tables:**
- 0% discount → **+$13.28K profit**
- 20% discount → approximately **-$304**
- 30% discount → **-$3.40K**
- 40% discount → **-$16.19K**
- 50% discount → **-$8.62K**

**Bookcases:**
- 0% discount → **+$6.08K profit**
- 15% discount → **+$1.42K**
- 20% discount → approximately **+$131**
- 30% discount → **-$556**
- 50% discount → **-$4.26K**
- 70% discount → **-$3.89K**

### 4. Central region needs attention

- Total sales: **$501.24K**
- Total profit: **$39.71K**
- Average discount: **24.04%**
- Central had the **highest average discount** and the **lowest total profit** among the four regions.

### 5. West is the strongest-performing region

- Total sales: **$725.46K**
- Total profit: **$108.42K**
- Average discount: **10.93%**
- West generated the **highest total profit** while maintaining a comparatively lower average discount.

## What-If Analysis

A Power BI What-If analysis was created to evaluate how changes in discount levels could affect profitability.

The interactive **Discount Scenario** parameter allows users to change the discount assumption and observe the resulting scenario profit.

This provides a simple way to evaluate potential discount decisions and understand their possible impact on profitability.

## Business Recommendations

Based on the analysis:

- Review and control excessive discounting, especially discounts of **30% or higher**.
- Review pricing and discount strategies for loss-making sub-categories such as **Tables and Bookcases**.
- Avoid applying large discounts to products or sub-categories with already weak margins.
- Investigate the **Central region's** pricing and discount strategy.
- Study the **West region** as a benchmark for stronger profitability with lower average discounting.
- Use What-If analysis to evaluate discount scenarios before making pricing decisions.
- Monitor loss-making sub-categories regularly to prevent continued margin erosion.

## Dashboard

The Power BI dashboard provides interactive analysis of:

- Sales and profit KPIs
- Category performance
- Segment performance
- Regional performance
- Discount vs. profit
- Sub-category profitability
- Profitability trends
- Business performance indicators

![Superstore Sales & Profit Analysis Dashboard](Superstore_Dashboard.png)

## What-If Analysis Dashboard

The What-If page allows users to adjust the discount scenario and observe changes in scenario profit.

![Discount What-If Analysis](Discount_What_If_Analysis.png)

## Project Structure

```text
Superstore Sales Profit Analysis/
│
├── Superstore_Sales_Profit_Dashboard.pbix
├── Superstore_Dashboard.png
├── Discount_What_If_Analysis.png
└── README.md
