# Churn Prediction – Problem Definition

## Business Problem
Customer churn is one of the biggest revenue risks for B2B SaaS companies.
Most churn signals appear in product usage data weeks before renewal.

The goal of this model is to identify accounts that are at high risk of churn
early enough for Customer Success teams to intervene.

---

## Prediction Target
Binary classification:
- 1 = Account is at risk of churn
- 0 = Account is healthy

---

## Input Features
The model uses explainable, product-driven features:
- Active Days (recent)
- Number of Active Users
- Number of Features Used
- Engagement Score
- Usage trend (increasing / decreasing)

---

## Model Objective
- Prioritize recall over precision
- Avoid false negatives (missing churn risks)
- Provide explainable predictions for business users

---

## How This Will Be Used
- Weekly churn risk review for Customer Success
- Targeted outreach for high-risk accounts
- Input into renewal forecasting
