# Advanced Data Modeling for Analytics: Retail & E‑commerce Case Study

## Table of Contents
- [Project Description](#project-description)
- [Aim & Objectives](#aim-and-objectives)
- [Methodology](#methodology)
- [Insights & Recommendations](#insights-and-recommendations)
- [Conclusion](#conclusion)

## Project Description
### This project explores advanced data modeling techniques to transform raw transactional data into a structured model suitable for analytics. Using Power BI and Python, the project builds a snowflake schema, performs correlation analysis, and develops interactive dashboards to uncover insights into sales, revenue drivers, customer sentiment, operations, and seller performance.

## Aim and Objectives
### Aim: To design and implement an advanced data model that supports comprehensive analytics and decision‑making.

Objectives:
#### - Structure the dataset into a snowflake schema with fact and dimension tables.
#### - Identify key fact and dimension tables.
#### - Analyze product categories and products generating highest/lowest revenue.
#### - Determine top 5 best‑performing products by sales and revenue.
#### - Explore sales trends over time.
#### - Examine the relationship between price, quantity sold, and revenue.
#### - Derive actionable insights and recommendations.
#### - Build an interactive dashboard in Power BI.

## ERD Overview

<img width="550" height="330" alt="Screenshot 2026-04-17 102107" src="https://github.com/user-attachments/assets/4dbcb7b1-9c56-4899-926a-a15a6910ab15" />

#### ERD Diagram


####  The ERD highlights the relationships between transactional data (facts) and descriptive data (dimensions). Instead of a simple star schema, i used a snowflake schema, normalizing dimension tables into multiple related tables. This reduces redundancy and improves data integrity. The model allowed me to connect the relationship between tables to be able to understand how they influence one another e.g Which product categories generate the highest revenue?”, “How does sentiment vary by seller type and fulfillment model?”, “Which campaigns drive the most sales?”

### Fact Tables
#### Key fact tables in this project includes;
- Orders table
- Order Item table
- Reviews table
- Shipments table

### Dimension Tables
#### These Include;
- Customers table
- Products table
- Sellers table
- Date table
- Location table

## Methodology
#### 1. Data Preparation – Cleaned, standardized data types and handled nulls.

#### 2. Data Normalization & ERD Design – Reviewed the entity–relationship diagram (ERD) to identify how Customers, Orders, Order Items, Products, Campaigns, Sellers, Reviews, Shipments, Date, and Location connect. Chose a snowflake schema to normalize dimensions (e.g., Customer → Location, Product → Campaign → Campaign Type).

#### 3. Data Modeling – 

- Defined Fact Tables: Orders, Order Items, Reviews, Shipments.

- Defined Dimension Tables: Customers, Products, Sellers, Campaigns, Date, Location.

- Established relationships to support queries.

#### 4. Hierarchies & Aggregation

- Built time hierarchies (Year → Quarter → Month → Day) for trend analysis.

- Created geographic hierarchies (Province → City → LocationID) for regional insights.

- Applied aggregation rules for revenue, gross profit, units sold, and Shipping duration averages.

#### 5. Data Transformation

- Encoded categorical variables:

- Seller type (Company = 1, Individual = 0).

- Fulfillment model (FBS = 1, Standard = 0).

- Product category (auto‑coded).

#### 6. Analysis – Applied Python for correlation analysis, Power BI for trend analysis and comparative analysis of product categories and seller regions..

#### 7. Visualization – Built dashboards for Sales, Revenue, Customers, Operations, and Sellers

## Insights and Recommendations

### A. Sales Insights
<img width="578" height="327" alt="Screenshot 2026-04-17 131054" src="https://github.com/user-attachments/assets/632718a8-78f4-45de-99e9-6fef1d194cbe" />


#### i. Growth Trend: Sales started low in 2022 but grew steadily, peaking in 2025 with revenue surpassing 2 billion.
#### ii. Cumulative Performance: Total revenue across the years is 4.7 billion, with gross profit at 3.7 billion. Nearly half of this came in 2025, showing strong momentum.
#### iii. Category Demand: Home products dominate both demand and revenue, indicating a strong consumer preference in this segment.

#### - Recommendations:
#### i. Double down on the Home category by expanding the product range and marketing campaigns.
#### ii. Investigate what drove the sharp growth in 2025 (campaigns, logistics, seller expansion) and replicate those strategies earlier in future cycles.
#### iii. Diversify categories to reduce over-reliance on Home, especially Electronics, which shows strong secondary demand.

### B. Revenue Insights

<img width="581" height="324" alt="Screenshot 2026-04-17 131210" src="https://github.com/user-attachments/assets/4abd4390-903e-4233-b944-28bc41d59ca5" />


#### i. Revenue Drivers: The top 7 products driving revenue are concentrated in Home and Electronics, confirming these as core revenue pillars.
#### ii. Campaign Impact: Campaign-linked products generated more than double the revenue of non-campaign products.
#### iii. Campaign Types: Flash sales are the most effective, followed by discounts, bundles, and vouchers.

#### - Recommendations:
#### i. Prioritise flash sales and discounts in campaign planning.
#### ii. Explore bundling strategies in Home and Electronics to increase basket size.
#### iii. Track ROI per campaign type to optimise marketing spend.

### C. Customer Insights

<img width="579" height="323" alt="Screenshot 2026-04-17 131258" src="https://github.com/user-attachments/assets/915ce1ef-58f8-4a89-867f-113ed34a02a3" />


#### i. Regional Distribution: Bangkok contributes the highest revenue, largely due to customer concentration.
#### ii. Sentiment Drivers: Reviews are more positive for electronics sold by companies, while Beauty/Groceries sold by individuals trend negative.
#### iii. Customer Value: Average revenue per customer is ~71 USD, with top customers generating significantly more.

#### - Recommendations:
#### i. Focus on retention and loyalty programmes in Bangkok to sustain revenue.
#### ii. Encourage individual sellers in Beauty/Groceries to improve quality and service standards.
#### iii. Segment customers by value (high vs. average spenders) and tailor promotions accordingly.

### D. Operations Insights

<img width="580" height="329" alt="Screenshot 2026-04-17 131354" src="https://github.com/user-attachments/assets/bd3305b1-6d32-4ea3-8a87-341ce30d0c65" />


#### i. Delivery Efficiency: Average delivery time is 34 hours (~1.5 days), which is strong compared to typical e-commerce benchmarks.
#### ii. Revenue tends to increase when average delivery time decreases
#### iii. Courier Performance: Some couriers outperform others in speed and reliability, directly influencing revenue.

#### - Recommendations:
#### i. Strengthen partnerships with top-performing couriers (e.g., Kerry Express, Best Express).

### E. Seller Insights

<img width="580" height="323" alt="Screenshot 2026-04-17 131434" src="https://github.com/user-attachments/assets/1d2fe2cd-8801-4eab-b5f9-29d84ab6e7f5" />


#### i. Seller Base: Out of 200 sellers, 180 are active, showing strong participation.
#### ii. Seller Type: Majority are companies (75%), with the Standard model (70%) dominating.

#### - Recommendations:
#### i. Support inactive sellers with onboarding and training to increase activity.
#### ii. Promote standard adoption further, as it correlates with higher revenue.


### Conclusion
#### 1. Sentiment vs. Fulfillment: Sellers using the standard model, tend to deliver faster and more reliably, which likely contributes to higher positive sentiment.
#### 2. Revenue Concentration: Heavy reliance on Bangkok and Home category suggests vulnerability, diversifying geographically and across categories would stabilize growth.
#### 3. Customer Reviews: With ~17% negative reviews, there’s room to improve customer experience, especially in Beauty and Groceries.

