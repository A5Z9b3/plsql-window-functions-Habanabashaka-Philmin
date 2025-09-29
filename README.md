
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

| Table       | Purpose          | Key Columns                              | Example Row                          |
|-------------|------------------|------------------------------------------|--------------------------------------|
| customers  | Customer info   | customer_id (PK), name, region          | 1001, Habanabashaka Philmin, Kigali |
| products   | Product catalog | product_id (PK), name, category         | 2001, Silver Fork Set, Silverware   |
| transactions | Sales records  | transaction_id (PK), customer_id (FK), product_id (FK), sale_date, amount | 3001, 1001, 2001, 2024-01-15, 15000 |

### ER Diagram 













### Combined Table Creation Image

![WhatsApp Image 2025-09-29 at 22 26 46_5ec25162](https://github.com/user-attachments/assets/b1f4ada0-b004-4c37-b9bc-63fc8ed95bec)

### Data inserting in customers

![WhatsApp Image 2025-09-29 at 21 39 27_7b906753](https://github.com/user-attachments/assets/0eb7d5c9-cee0-4462-af14-cf45034cda91)

### Data inserting in products

![WhatsApp Image 2025-09-29 at 21 39 28_b4594a93](https://github.com/user-attachments/assets/04535e01-37e2-475d-a5d2-e6ef476fdac5)


### Data inserting in transactions

![WhatsApp Image 2025-09-29 at 21 39 28_c2b06434](https://github.com/user-attachments/assets/2590c057-e96a-474c-84c6-a5859ce86dd9)


## Window Functions Implementation

1. Ranking: ROW_NUMBER(), RANK(), DENSE_RANK(), PERCENT_RANK()


![WhatsApp Image 2025-09-29 at 21 39 27_457cae98](https://github.com/user-attachments/assets/b30c06b1-e142-46c9-9a23-05be96eb60c4)



2. Aggregate: SUM(), AVG(), MIN(), MAX() with frame comparisons (ROWS vs RANGE)


![WhatsApp Image 2025-09-29 at 21 39 32_fbc99960](https://github.com/user-attachments/assets/44a00141-a598-4414-93f6-50f6b432b5bb)



3. Navigation: LAG(), LEAD(), growth % calculations

![WhatsApp Image 2025-09-29 at 21 39 27_f2116755](https://github.com/user-attachments/assets/f18e2070-a73a-4e9c-9ee6-bd03813355bf)




4. Distribution: NTILE(4), CUME_DIST()
![WhatsApp Image 2025-09-29 at 21 39 28_858b33a6](https://github.com/user-attachments/assets/d9ce5ade-4f22-4d6c-a244-ff4fffe94730)




## Results Analysis
1. Descriptive – What happened?
Sales peaked in May at 27,000 RWF with Silver Fork Set as the top product in Kigali and Musanze. Trends show overall growth from January to May, then a dip in June. Outliers include high individual transactions in Musanze.
2. Diagnostic – Why?
The growth in April-May could be due to seasonal demand for kitchenware during family events in Rwanda. Comparisons show Kigali customers spend more frequently, possibly due to urban market access, while lower segments in Huye indicate competition or economic factors.
3. Prescriptive – What next?
Prioritize marketing to quartile 1 customers with discounts on top products like Silver Fork Set. Stock more in high-growth regions like Kigali and monitor 3-month averages to predict inventory needs. Implement targeted campaigns for lower quartiles to boost frequency.

### References

- YouTube Tutorial: Git Tutorial for Beginners: Learn Git in 1 Hour (from Lecture02 Introduction to GitHub.pdf)
- GitHub and Git Tutorial for Beginners (from Lecture - 02 Introduction to GitHub.pdf)
- Introduction to GitHub (from Lecture - 02 Introduction to GitHub.pdf)
- Intro to GitHub for version control (from Lecture - 02 Introduction to GitHub.pdf)
- How to Design an Attractive GitHub Profile Readme (from Lecture - 02 Introduction to GitHub.pdf)
- YouTube Tutorial: How to create Professional Github Readme Profile (Step By Step) (from Lecture - 02 Introduction to GitHub.pdf)
- Getting Started with R Markdown (from Lecture - 02 Introduction to GitHub.pdf)
- YouTube Tutorial: Git Merge Conflicts (from Lecture - 02 Introduction to GitHub.pdf)
- SQL Window Functions (from Lecture - 01 Introduction to SQL Command Basics (Recap).pdf)
- Oracle PL/SQL Documentation: Window Functions (adapted from course outline in Lecture - 00 Course Introduction.pdf)

### All sources were properly cited. Implementations and analysis represent original work. No AI generated content was copied without attribution or adaptation.









