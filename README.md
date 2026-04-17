# Advanced Data Modeling for Analytics: Retail & E‑commerce Case Study

## Project Description
### This project explores advanced data modeling techniques to transform raw transactional, customer, and seller data into a structured model suitable for analytics. Using Power BI and Python, the project builds a star schema, performs correlation analysis, and develops interactive dashboards to uncover insights into sales, revenue drivers, customer sentiment, operations, and seller performance.

## Aim and Objectives
### Aim: To design and implement an advanced data model that supports comprehensive analytics and decision‑making.

Objectives:
#### - Structure the dataset into a star schema with fact and dimension tables.
#### - Identify key fact and dimension tables.
#### - Analyze product categories and products generating highest/lowest revenue.
#### - Determine top 5 best‑performing products by sales and revenue.
#### - Explore sales trends over time.
#### - Examine the relationship between price, quantity sold, and revenue.
#### - Derive actionable insights and recommendations.
#### - Build an interactive dashboard in Power BI.

## Processes
#### 1. Data Understanding – Reviewed ERD and identified relationships between customers, orders, reviews, products, campaigns, sellers, and shipments.

#### 2. Data Modeling – Designed a star schema:

Fact tables: Orders, Order Items, Reviews, Shipments.

Dimension tables: Customers, Products, Sellers, Campaigns, Date, Location.

#### 3. Data Preparation – Cleaned and merged tables, encoded categorical variables, handled nulls.

#### 4. Analysis – Applied Python for correlation analysis and Power BI for trend analysis.

#### 5. Visualization – Built dashboards for Sales, Revenue, Customers, Operations, and Sellers

## Insights and Recommendations

### Sales Insights

#### Growth Trend: Sales started low in 2022 but grew steadily, peaking in 2025 with revenue surpassing 2 billion.
Cumulative Performance: Total revenue across the years is 4.7 billion, with gross profit at 3.7 billion. Nearly half of this came in 2025, showing strong momentum.
#### Category Demand: Home products dominate both demand and revenue, indicating a strong consumer preference in this segment.

#### - Recommendations:
#### - Double down on the Home category by expanding the product range and marketing campaigns.
#### - Investigate what drove the sharp growth in 2025 (campaigns, logistics, seller expansion) and replicate those strategies earlier in future cycles.
#### - Diversify categories to reduce over-reliance on Home, especially Electronics, which shows strong secondary demand.

### Revenue Insights
#### Revenue Drivers: The top 7 products driving revenue are concentrated in Home and Electronics, confirming these as core revenue pillars.
#### Campaign Impact: Campaign-linked products generated more than double the revenue of non-campaign products.
#### Campaign Types: Flash sales are the most effective, followed by discounts, bundles, and vouchers.

#### - Recommendations:
#### Prioritise flash sales and discounts in campaign planning.
#### Explore bundling strategies in Home and Electronics to increase basket size.
#### Track ROI per campaign type to optimise marketing spend.

### Customer Insights
#### Regional Distribution: Bangkok contributes the highest revenue, largely due to customer concentration.
#### Sentiment Drivers: Reviews are more positive for electronics sold by companies, while Beauty/Groceries sold by individuals trend negative.
#### Customer Value: Average revenue per customer is ~71 USD, with top customers generating significantly more.

#### - Recommendations:
#### Focus on retention and loyalty programmes in Bangkok to sustain revenue.
#### Encourage individual sellers in Beauty/Groceries to improve quality and service standards.
#### Segment customers by value (high vs. average spenders) and tailor promotions accordingly.

### Operations Insights
#### Delivery Efficiency: Average delivery time is 34 hours (~1.5 days), which is strong compared to typical e-commerce benchmarks.
#### Courier Performance: Some couriers outperform others in speed and reliability, directly influencing revenue.

#### - Recommendations:
#### Strengthen partnerships with top-performing couriers (e.g., Kerry Express, Best Express).

### Seller Insights
#### Seller Base: Out of 200 sellers, 180 are active, showing strong participation.
#### Seller Type: Majority are companies (75%), with the Standard model (70%) dominating.

#### - Recommendations:
#### Support inactive sellers with onboarding and training to increase activity.
#### Promote standard adoption further, as it correlates with higher revenue.


### Conclusion
#### - Sentiment vs. Fulfillment: FBS sellers tend to deliver faster and more reliably, which likely contributes to higher positive sentiment.
#### - Revenue Concentration: Heavy reliance on Bangkok and Home category suggests vulnerability — diversifying geographically and across categories would stabilize growth.
#### - Customer Reviews: With ~17% negative reviews, there’s room to improve customer experience, especially in Beauty and Groceries.

