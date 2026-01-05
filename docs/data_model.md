# Product Intelligence Platform – Data Model

## 1. Product Context
This project simulates a B2B SaaS product similar to Planview, serving mid-market
and enterprise customers with account-based licensing and multiple user roles.

The goal is to unify product usage, revenue, and customer health data to:
- Predict churn risk before renewal
- Identify expansion opportunities
- Measure real feature adoption
- Enable data-driven product and customer success decisions

---

## 2. Design Principles
- Account-centric analytics
- Event-based product usage tracking
- Scalable to thousands of customers
- Supports product, CSM, and executive use cases

---

## 3. Data Grains
- Event grain: One row per user action
- User grain: One row per user
- Account grain: One row per customer
- Feature grain: One row per feature per account per day

---

## 4. Core Tables

### Dimensions
- dim_account
- dim_user
- dim_feature
- dim_date

### Fact Tables
- fact_product_events
- fact_feature_usage_daily
- fact_account_metrics_daily
- fact_revenue
- fact_support_tickets

---

## 5. Why This Model Works
This model allows:
- Accurate measurement of engagement and adoption
- Attribution of churn and expansion to product behavior
- Clear ownership of metrics across teams
- Easy extension into machine learning models
