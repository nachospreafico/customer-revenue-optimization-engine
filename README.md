# Customer Revenue Optimization Engine

_An End-to-End Data Science Project for ROI-Driven Customer Retention Decisions_

---

## Executive Summary

Businesses often build churn prediction models, but knowing _who is likely to churn_ is only part of the problem. The real business challenge is deciding **which customers should be targeted, with what limited budget, and where intervention will generate the highest financial return**.

This project reframes customer retention as a business decision optimization problem rather than a purely predictive machine learning task. Using customer, demographic, service usage, and revenue data from a telecommunications company, the project develops an end-to-end data science solution that combines analytics, predictive modeling, and business optimization to maximize the expected return on retention campaigns.

The final solution delivers actionable recommendations through an interactive decision engine and executive dashboard, demonstrating how data science can move beyond prediction to directly support strategic business decisions.

---

## Project Objectives

The objective of this project is to design and develop an end-to-end decision support system that enables a business to maximize the return on customer retention initiatives.

Specifically, the project aims to:

- Build a production-style analytical data model from raw customer data.
- Explore customer behavior through exploratory data analysis (EDA) and business-driven metrics.
- Engineer predictive features using SQL and Python.
- Develop machine learning models to estimate customer churn risk.
- Estimate the expected business value of customer retention actions.
- Prioritize customers based on expected return on investment (ROI) under budget constraints.
- Deliver recommendations through an executive dashboard designed for business stakeholders.
- Demonstrate an end-to-end data science workflow, from business understanding to actionable recommendations.

---

## Business Context

A telecommunications company is experiencing increasing customer churn while operating under a limited retention budget. Although historical customer data is available, existing retention efforts rely primarily on broad campaigns rather than data-driven decision making.

The business objective is not simply to identify customers who are likely to churn, but to determine **which customers should be targeted first to maximize the financial return of retention initiatives**.

This project assumes the role of a Data Scientist tasked with designing a decision support system capable of transforming customer data into actionable business recommendations. Rather than optimizing predictive performance alone, the solution focuses on supporting strategic decisions that improve customer retention while maximizing expected business value.

---

## Dataset

This project uses the **IBM Telco Customer Churn (11.1.3+)** dataset, a realistic telecommunications dataset containing customer demographics, account information, subscribed services, usage characteristics, billing details, and customer retention indicators.

The dataset provides sufficient information to simulate a real-world customer retention initiative by combining historical customer behavior with financial and operational attributes.

Key data domains include:

- Customer demographics
- Geographic information
- Account and contract details
- Service subscriptions
- Internet and phone services
- Billing and payment information
- Customer lifetime value (CLTV)
- Churn labels and churn-related metrics

The multi-table structure closely resembles an operational business database, making it well suited for demonstrating SQL data modeling, feature engineering, predictive analytics, and business decision optimization within a realistic end-to-end data science workflow.

---

# Project Architecture

The project follows an end-to-end data science workflow that transforms raw operational data into business recommendations for customer retention.

```
                    ┌─────────────────────┐
                    │   Raw Source Data   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   SQL Data Model    │
                    │ Data Cleaning & ETL │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Exploratory Data    │
                    │ Analysis (EDA)      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Feature Engineering │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Machine Learning    │
                    │ Churn Prediction    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Business Decision   │
                    │ Optimization        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Executive Dashboard │
                    │ & Recommendations   │
                    └─────────────────────┘
```

Each stage produces an independent deliverable while serving as the foundation for the next phase, reflecting a production-oriented data science workflow from raw data to business decision support.
