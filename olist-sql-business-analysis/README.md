# E-Commerce Business Analysis

## Project Overview

This project uses PostgreSQL and SQL to analyze approximately 100,000 orders from the Brazilian e-commerce marketplace Olist.

The analysis examines revenue trends, customer purchasing behavior, product category performance, geographic markets, seller performance, and the relationship between delivery performance and customer reviews.

The goal was to use SQL to answer practical business questions while maintaining appropriate data grain across a relational dataset containing multiple interconnected tables.

---

## Tools & Skills

- PostgreSQL
- SQL
- pgAdmin
- Excel
- Relational Data
- JOINs
- Common Table Expressions (CTEs)
- Window Functions
- LAG
- RANK
- CASE Statements
- Aggregations
- Subqueries
- Date Analysis
- Data Grain Validation
- Business Analysis

---

## Business Objective

The analysis was designed to investigate questions such as:

- How has revenue changed over time?
- Which product categories contribute the most revenue?
- Which geographic markets generate the greatest sales?
- How common are repeat customers?
- Which sellers contribute the most marketplace revenue?
- Is marketplace revenue highly concentrated among a small number of sellers?
- How long does delivery typically take?
- How does delivery performance relate to customer review scores?

---

## Data Structure & Analytical Approach

The source data is distributed across multiple relational tables containing information about:

- Orders
- Customers
- Order items
- Products
- Sellers
- Payments
- Reviews
- Geolocation
- Product category translations

Rather than creating one large joined table for every analysis, queries were structured around the appropriate grain for each business question.

This approach helped prevent one-to-many relationships between orders, items, payments, and reviews from unintentionally duplicating records or inflating calculated results.

---

## Revenue & Growth

Revenue analysis was used to evaluate historical performance and month-over-month changes.

<img width="988" height="1234" alt="image" src="https://github.com/user-attachments/assets/4cc7dcce-951d-4ca0-8be6-66334b58325a" />
<img width="940" height="1164" alt="image" src="https://github.com/user-attachments/assets/2208d2a8-a9c6-4f0a-854a-c49c9e09bd22" />


The analysis identified substantial growth during the dataset's primary operating period, including a significant increase in revenue between October and November 2017.

Following this increase, monthly revenue generally remained at a higher level than during the earlier periods in the dataset.

---

## Product Category Performance

Product category analysis was used to identify the categories contributing the greatest merchandise revenue and examine changes in category leadership over time.

<img width="946" height="1284" alt="image" src="https://github.com/user-attachments/assets/a04ef54e-ca4a-4ec1-8928-195fcfc3840a" />

Historically, several categories represented major contributors to marketplace revenue, including Health & Beauty, Watches & Gifts, Bed Bath & Table, Sports & Leisure, and Computers & Accessories.

---

## Customers & Geographic Markets

Customer and geographic analysis examined purchasing activity across Brazilian states and the frequency of repeat purchasing.

<img width="982" height="1066" alt="image" src="https://github.com/user-attachments/assets/5fd4e6a3-b4a8-404d-a480-de5e2a73b4c7" />
<img width="952" height="1218" alt="image" src="https://github.com/user-attachments/assets/f4dc306f-db85-49a8-97fd-5827a21a6c0f" />


São Paulo represented the largest geographic market by revenue within the dataset.

Repeat purchasing was relatively uncommon, with approximately 3% of identified customers placing more than one order.

---

## Seller Performance

Seller analysis examined marketplace revenue concentration and the contribution of leading sellers.

<img width="972" height="944" alt="image" src="https://github.com/user-attachments/assets/4fc37d08-0247-49c4-adb1-d32da06ace39" />
<img width="946" height="900" alt="image" src="https://github.com/user-attachments/assets/1c7188ed-f9ae-400a-91ee-2ee2378b220f" />


The top 10 sellers represented approximately 13% of merchandise revenue, indicating that marketplace revenue was not highly concentrated among only the largest sellers.

---

## Delivery & Customer Experience

Delivery performance was analyzed alongside customer review scores to investigate the relationship between fulfillment speed and reported customer experience.

<img width="950" height="1186" alt="image" src="https://github.com/user-attachments/assets/f682d484-c779-49a4-a37d-d4a1c800ab71" />
<img width="818" height="1298" alt="image" src="https://github.com/user-attachments/assets/876d1657-19b5-4a02-b2ea-edf17973887b" />


Average delivery time increased as review scores declined:

- 5-star reviews: approximately 10 days
- 4-star reviews: approximately 11 days
- 3-star reviews: approximately 13 days
- 2-star reviews: approximately 16 days
- 1-star reviews: approximately 20 days

Orders delivered on time also received substantially higher average review scores than late orders.

These results identify a strong relationship within the dataset between delivery performance and customer satisfaction, although the analysis does not by itself establish causation.

---

## Key SQL Techniques

The analysis incorporates:

- Multi-table JOINs
- Aggregate functions
- Common Table Expressions
- Window functions
- Ranking
- LAG for period-over-period analysis
- CASE expressions
- Subqueries
- Date calculations
- Distinct customer and order analysis
- Data grain validation

---

## Project Outcome

The completed analysis demonstrates how SQL can be used to investigate business performance across a complex relational dataset while maintaining awareness of table relationships and analytical grain.

The project combines technical SQL querying with business-focused analysis across revenue, customers, products, sellers, geography, delivery performance, and customer experience.

---

## Data Source

This project uses the Brazilian E-Commerce Public Dataset by Olist.

The dataset was used for portfolio and educational purposes.

---

## SQL

The SQL queries used throughout this analysis are available in this project folder:

`analysis.sql`
