# Project Design Document

## Project Overview

**Project Name:** Customer Revenue Optimization Engine

**Objective:** Build an end-to-end data science solution that transforms
customer data into actionable retention decisions by combining
analytics, predictive modeling, and business optimization.

------------------------------------------------------------------------

# Business Problem

A telecommunications company experiences customer churn while operating
under a limited retention budget.

Rather than identifying customers who are likely to churn, the goal is
to determine which customers should be targeted to maximize the expected
return on investment (ROI) of retention campaigns.

------------------------------------------------------------------------

# Business Objectives

-   Reduce customer churn.
-   Maximize retention ROI.
-   Prioritize high-value customers.
-   Support executive decision-making through analytics.

------------------------------------------------------------------------

# Stakeholders

-   Executive Leadership
-   Marketing
-   Customer Success
-   Finance
-   Data Science & Analytics

------------------------------------------------------------------------

# Project Scope

## In Scope

-   SQL data modeling
-   Exploratory Data Analysis
-   Feature Engineering
-   Churn prediction
-   Decision optimization
-   Power BI dashboard
-   Executive recommendations

## Out of Scope

-   Production deployment
-   Real-time inference
-   MLOps infrastructure
-   Cloud deployment

------------------------------------------------------------------------

# Success Criteria

## Business

-   Prioritize customers by expected business value.
-   Demonstrate improved retention decision-making under budget
    constraints.

## Technical

-   Reproducible pipeline
-   Well-documented SQL transformations
-   Robust predictive model
-   Explainable results
-   Interactive dashboard

------------------------------------------------------------------------

# Data Sources

Primary dataset:

-   IBM Telco Customer Churn (11.1.3+)

Expected domains:

-   Demographics
-   Geography
-   Contracts
-   Services
-   Billing
-   Payments
-   Customer Lifetime Value
-   Churn

------------------------------------------------------------------------

# High-Level Workflow

1.  Data Understanding
2.  SQL Data Model
3.  Exploratory Data Analysis
4.  Feature Engineering
5.  Predictive Modeling
6.  Decision Optimization
7.  Executive Dashboard
8.  Business Recommendations

------------------------------------------------------------------------

# Modeling Strategy

Primary task:

-   Binary classification (Churn)

Candidate models:

-   Logistic Regression
-   Random Forest
-   XGBoost

Evaluation:

-   ROC-AUC
-   Precision
-   Recall
-   F1 Score
-   Confusion Matrix

Business evaluation:

-   Expected retained revenue
-   Customer prioritization quality
-   Estimated ROI

------------------------------------------------------------------------

# Dashboard Vision

The dashboard should answer:

-   What is the current churn situation?
-   Who are the highest-risk customers?
-   Which customers should be contacted first?
-   What is the expected business impact?
-   How does ROI change under different budget scenarios?

------------------------------------------------------------------------

# Risks & Assumptions

## Risks

-   Dataset limitations
-   Missing variables
-   Simplified business assumptions

## Assumptions

-   Historical churn is representative.
-   CLTV is a suitable proxy for customer value.
-   Budget constraints are fixed during optimization.

------------------------------------------------------------------------

# Deliverables

-   SQL data model
-   EDA notebook
-   Feature engineering pipeline
-   Predictive model
-   Decision Optimization Engine
-   Power BI dashboard
-   Executive presentation
-   GitHub repository

------------------------------------------------------------------------

# Milestones

-   Business Understanding & Design
-   Data Understanding
-   SQL Data Model
-   Exploratory Data Analysis
-   Feature Engineering
-   Predictive Modeling
-   Decision Optimization
-   Executive Dashboard
-   Business Recommendations
-   Executive Presentation

------------------------------------------------------------------------

# Guiding Principle

**The objective is not to build the most accurate churn model, but to
build the best decision-support system for maximizing customer retention
ROI.**
