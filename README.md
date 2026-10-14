# Retail Profitability & Customer Behaviour Analysis

**Author:** Afsana Yeasmin Ahona    
**Role:** Aspiring Data Analyst    
**Tools:** Python, Pandas, Matplotlib, Google Colab

## Project Overview
This project analyzes retail sales data to identify profitability trends, evaluate discount strategies, and highlight underperforming product categories. The analysis uses Python to clean data, investigate business performance, and create visualizations that support data-driven recommendations. 

## Objectives
	•	Assess overall sales and profitability.
	•	Compare performance across product categories and sub-categories.
	•	Investigate the relationship between discount levels and profit margins.
	•	Examine customer purchasing patterns and returned orders.
	•	Translate findings into practical business recommendations.
## Tools & Technologies
	•	Python — data analysis and calculations
	•	Pandas — data cleaning, grouping, and aggregation
	•	Matplotlib — data visualisation
	•	Google Colab — notebook development and execution
## Dataset & Data Quality
The dataset contains 9,994 transaction rows and 21 columns, covering order dates, shipping information, customers, products, sales, discounts, and profit.
Initial quality checks identified:
	•	0 exact duplicate rows
	•	11 missing postal codes
	•	1,871 transactions with negative profit
	•	800 return records representing 296 unique returned order IDs
The original data was preserved during analysis. Missing postal codes and loss-making transactions were retained rather than removed without justification. Return records were deduplicated by order ID when creating the returned-order flag.
## Key Findings
	•	Total sales: $2,297,200.86
	•	Total profit: $286,397.02
	•	Overall profit margin: approximately 12.47%
	•	Orders: 5,009 unique order IDs
	•	Customers: 793 unique customer IDs
Technology generated the highest sales and profit among the three product categories. Office Supplies also delivered strong overall profit, while Furniture generated substantial sales but comparatively low profit.
At the sub-category level, Copiers, Phones, and Accessories were leading profit contributors. Tables recorded a net loss of $17,725.48, while Bookcases recorded a net loss of $3,472.56.
The discount analysis also showed negative aggregate profit margins at several higher discount levels for Tables and Bookcases. These patterns warrant further investigation into pricing, costs, and discount policies.

## Recommendations

1. Review pricing, product costs, and discount policies for loss-making sub-categories.
2. Evaluate high-discount transactions to determine where margins deteriorate.
3. Monitor profit margins alongside sales growth rather than relying on revenue alone.
4. Investigate product-level and customer-level performance before implementing changes.
5. Track returned orders and assess their relationship with profitability.

## Visualizations

### 1. Monthly Sales and Profit
Shows monthly sales and profit trends from 2018 to 2021, highlighting fluctuations in business performance.

![Monthly Sales and Profit](visuals/monthly_sales_profit.png)

### 2. Profit by Product Subcategory
Compares profitability across product subcategories, identifying strong contributors and loss-making areas.

![Profit by Subcategory](visuals/profit_by_subcategory.png)

### 3. Sales by Category
Compares total sales across Furniture, Office Supplies, and Technology.

![Sales by Category](visuals/sales_by_category.png)

### 4. Discount Level vs. Profit Margin
Examines the relationship between discount levels and profit margins for Tables and Bookcases.

![Discount vs. Profit Margin](visuals/discount_vs_profit_margin.png)

## Project Files
	•	01_data_quality_audit.ipynb — analysis, data quality checks, tables, and visualisations
	•	superstore_business_findings.csv — summary of key findings and recommendations
	•	visuals/ — exported chart images

## Limitations
This analysis identifies patterns and associations in historical transaction data. It does not establish that discounts caused losses, nor does it quantify the financial impact of the recommendations. Further analysis would be required to test specific pricing changes and assess their effects.
