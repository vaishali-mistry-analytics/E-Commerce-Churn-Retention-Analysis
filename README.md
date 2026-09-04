# 🛒 E-Commerce Churn-Risk & Retention Analysis using MySQL

A portfolio data analytics project that uses SQL to analyze e-commerce customer behavior, purchasing patterns, revenue, customer segments, and rule-based churn risk.

> **Important:** This project uses synthetic data. The analysis identifies churn-risk / at-risk customers using business rules; it does not calculate a statistically validated historical churn rate or build a machine-learning churn model.

## 🎯 Business Objective

The goal is to convert customer, order, product, activity, and support data into actionable retention insights.

The project focuses on:

- Customer and order KPIs
- Revenue and Average Order Value
- Monthly revenue trends
- Product and category performance
- Repeat vs one-time customers
- Customer recency and purchase frequency
- RFM-style segmentation
- Rule-based at-risk customer identification
- Risk comparison across membership tiers, devices, and preferred categories
- Support interaction analysis
- Customer revenue contribution
- Return and cancellation rates

## ❓ Business Questions

1. How many customers and orders are in the dataset?
2. What is completed revenue and Average Order Value?
3. How does revenue change month by month?
4. Which product categories generate the most revenue and profit?
5. How many customers are repeat buyers?
6. Which customers have high purchase recency risk?
7. Which customer segments are high-value or at risk?
8. Which membership tiers and devices have higher risk rates?
9. Which products generate the most revenue?
10. What percentage of orders are cancelled or returned?
11. Which customers have high support interaction volume?
12. Which customers contribute the most revenue?

## 🗂️ Dataset

| Table | Rows | Purpose |
|---|---:|---|
| customers | 1,500 | Customer profile and membership information |
| products | 100 | Product, category, price and cost |
| orders | 4,500 | Customer orders and order status |
| order_items | 11,218 | Products purchased in each order |
| customer_activity | 1,500 | Recency and recent activity |
| support_interactions | 2,200 | Customer support history |

## 🧩 Database Schema

```text
customers
   │
   ├── orders
   │      │
   │      └── order_items ─── products
   │
   ├── customer_activity
   │
   └── support_interactions
