# Dashboard Plan

## Dataset
Use the retail sales dataset from the `data-analysis-project` repository.

## Page 1 — Executive Overview

### KPI Cards
- Total Sales
- Total Profit
- Profit Margin
- Total Units

### Visuals
- Monthly Sales Trend
- Sales by Category
- Sales by Region

### Slicers
- Region
- Category
- Subcategory
- Order Date

## Page 2 — Product & Profitability

- Sales and profit by subcategory
- Profit margin by category
- Discount vs. profit analysis
- Top products/subcategories by sales

## Suggested DAX Measures

```DAX
Total Sales = SUM(Sales[Sales])

Total Profit = SUM(Sales[Profit])

Total Units = SUM(Sales[Units])

Profit Margin = DIVIDE([Total Profit], [Total Sales])

Average Order Value = AVERAGE(Sales[Sales])
```

## Design Principles

- Keep the dashboard focused on business questions.
- Avoid unnecessary charts and decoration.
- Use consistent labels and number formatting.
- Make the most important KPIs immediately visible.
- Add short insight text where it improves interpretation.
