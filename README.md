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

## Project Architecture

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

---

## Tech Stack

| Category                | Technologies                         |
| ----------------------- | ------------------------------------ |
| Programming             | Python                               |
| Data Processing         | pandas, NumPy                        |
| SQL                     | SQL Server                           |
| Machine Learning        | scikit-learn, XGBoost                |
| Data Visualization      | Matplotlib, Power BI                 |
| Development Environment | Jupyter Notebook, Visual Studio Code |
| Version Control         | Git, GitHub                          |
| Project Management      | GitHub Projects                      |

---

## Repository Structure

```text
customer-revenue-optimization-engine/
│
├── data/               # Raw and processed datasets
├── notebooks/          # Exploratory analysis and model development
├── sql/                # Database schema, queries, views, and feature engineering
├── src/                # Reusable Python modules
├── dashboard/          # Power BI dashboard files
├── docs/               # Project documentation and diagrams
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Project Roadmap

The project is developed incrementally, with each milestone delivering a complete and measurable business outcome while serving as the foundation for subsequent phases.

| Milestone                                  | Status | Deliverable                                                 |
| ------------------------------------------ | :----: | ----------------------------------------------------------- |
| 1. Business Understanding & Project Design |   ⏳   | Define business objectives, architecture, and project scope |
| 2. Data Understanding                      |   ⏳   | Explore the dataset and assess data quality                 |
| 3. SQL Data Model                          |   ⏳   | Build a production-style analytical data model              |
| 4. Exploratory Data Analysis (EDA)         |   ⏳   | Identify customer behavior patterns and business insights   |
| 5. Feature Engineering                     |   ⏳   | Create predictive features using SQL and Python             |
| 6. Churn Prediction Model                  |   ⏳   | Train and evaluate machine learning models                  |
| 7. Customer Value Estimation               |   ⏳   | Estimate customer lifetime value and business impact        |
| 8. Decision Optimization Engine            |   ⏳   | Prioritize retention actions based on expected ROI          |
| 9. Executive Dashboard                     |   ⏳   | Build an interactive Power BI dashboard for stakeholders    |
| 10. Business Recommendations               |   ⏳   | Deliver actionable insights and strategic recommendations   |

---

## Data Model

The analytical data model is designed to transform raw operational data into a clean, analysis-ready structure that supports exploratory analysis, feature engineering, machine learning, and business decision optimization.

The model follows a relational design that consolidates customer, demographic, geographic, service, billing, and churn information into a unified analytical dataset while preserving data integrity and minimizing redundancy.

Key objectives of the data model include:

- Standardize and clean raw source data.
- Establish relationships between business entities.
- Create reusable SQL views for downstream analysis.
- Produce a single analytical dataset for feature engineering and model development.
- Ensure reproducibility through SQL-first data transformations.

The resulting data model serves as the single source of truth for all subsequent stages of the project, from exploratory data analysis to the final decision optimization engine.

> **Note:** The complete database schema, SQL scripts, and analytical views are available in the `/sql` directory.

---

## Exploratory Data Analysis

The exploratory data analysis (EDA) phase focuses on understanding customer behavior, identifying key business patterns, assessing data quality, and uncovering insights that guide feature engineering and predictive modeling.

Rather than exploring the data in isolation, the analysis is driven by business-oriented questions, including:

- Which customer segments exhibit the highest churn rates?
- How do contract type, tenure, and subscribed services influence customer retention?
- Which payment methods and billing characteristics are associated with increased churn?
- How does customer lifetime value vary across different customer segments?
- Are there identifiable behavioral patterns that distinguish retained customers from those who churn?
- Which variables are likely to provide the greatest predictive value for downstream machine learning models?

The findings from this phase directly inform feature engineering, model selection, and the business assumptions underlying the decision optimization engine.

> **Deliverables**
>
> - Data quality assessment
> - Descriptive statistics
> - Univariate and multivariate analysis
> - Correlation analysis
> - Customer segmentation
> - Business insights and recommendations

---

## Feature Engineering

Feature engineering transforms raw customer data into meaningful predictive variables that better capture customer behavior and improve model performance.

Rather than relying solely on the original dataset, this phase focuses on creating business-driven features that represent customer engagement, contractual relationships, service usage, and financial characteristics.

Feature engineering activities include:

- Data cleaning and preprocessing
- Handling missing values
- Encoding categorical variables
- Feature scaling where appropriate
- Creation of derived business metrics
- Identification and treatment of outliers
- Feature selection based on statistical and business relevance

The objective is to produce a high-quality analytical dataset that balances predictive performance with interpretability, ensuring that the resulting models remain both accurate and actionable for business stakeholders.

> **Deliverables**
>
> - Clean modeling dataset
> - Engineered predictive features
> - Feature importance assessment
> - Data preprocessing pipeline
> - Reproducible feature engineering workflow

---

## Predictive Modeling

The predictive modeling phase estimates each customer's likelihood of churn using supervised machine learning techniques.

Multiple classification algorithms are developed, compared, and evaluated to identify the best balance between predictive performance, robustness, and interpretability. Model selection is based not only on statistical performance but also on its ability to support downstream business decisions.

The modeling workflow includes:

- Baseline model development
- Model training and hyperparameter tuning
- Cross-validation
- Performance evaluation
- Model comparison
- Feature importance and model explainability

Models are evaluated using business-relevant performance metrics, ensuring that predictive accuracy translates into practical value for customer retention initiatives.

> **Deliverables**
>
> - Baseline model
> - Optimized predictive model
> - Model evaluation report
> - Feature importance analysis
> - Model explainability

---

## Decision Optimization Engine

Predicting customer churn is only the first step. The primary objective of this project is to transform predictive insights into actionable business decisions.

The Decision Optimization Engine combines model predictions with business constraints to identify the customer retention strategy expected to generate the greatest financial return.

Instead of ranking customers solely by churn probability, the engine prioritizes retention opportunities based on their estimated business value, enabling more efficient allocation of limited marketing resources.

The optimization framework considers multiple decision factors, including:

- Predicted probability of churn
- Estimated customer lifetime value (CLTV)
- Expected financial impact of customer loss
- Retention campaign budget constraints
- Estimated return on investment (ROI)

The final output is a prioritized list of customers ranked by expected business value, allowing decision-makers to maximize the effectiveness of retention campaigns while operating within realistic business constraints.

> **Deliverables**
>
> - Customer prioritization engine
> - ROI-based customer ranking
> - Budget allocation scenarios
> - Retention opportunity analysis
> - Executive decision recommendations

---
