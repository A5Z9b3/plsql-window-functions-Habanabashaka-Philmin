
# PL/SQL ASSIGNMENT

# INTRODUCTION

- NAMES:HABANABASHAKA PHILMIN
- ID:27487
- GROUP :A



# PL/SQL Window Functions  Project

## Problem Definition
### Business Context
Company type: Small family kitchenware retail business (Rwanda Kitchen Essentials Ltd.), Department: Sales and Inventory, Industry: Retail and Household Goods in Rwanda.

### Data Challenge
The company sells table silverware and kitchen stuff across regions in Rwanda, but the team faces issues in ranking top-selling products by region, monitoring monthly sales trends, calculating growth rates, and segmenting customers by spending levels. This leads to difficulties in optimizing stock and planning family-targeted promotions without detailed analysis.

### Expected Outcome
The analysis will deliver insights like top products per region, running sales totals with growth percentages, and customer segments in quartiles to support better inventory decisions and marketing for family households.


## Step 3: Database Schema
Design minimum 3 related tables with foreign keys.

| Table       | Purpose          | Key Columns                              | Example Row                          |
|-------------|------------------|------------------------------------------|--------------------------------------|
| customers  | Customer info   | customer_id (PK), name, region          | 1001, Habanabashaka Philmin, Kigali |
| products   | Product catalog | product_id (PK), name, category         | 2001, Silver Fork Set, Silverware   |
| transactions | Sales records  | transaction_id (PK), customer_id (FK), product_id (FK), sale_date, amount | 3001, 1001, 2001, 2024-01-15, 15000 |

### ER Diagram (Text-Based Representation)
