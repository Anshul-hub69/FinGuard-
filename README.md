# FinGuard – Predictive Analysis of Financial Consumer Complaints

**Predictive Analysis of Financial Consumer Complaints and Company Response Outcomes Using Machine Learning**

FinGuard is a machine learning and data analysis project that studies consumer complaints related to financial products, particularly money transfers, virtual currency, and mobile wallets. It explores complaint patterns, identifies common issues, examines company response outcomes, and builds predictive models to classify whether companies provide timely responses.

The project uses the **Consumer Financial Protection Bureau (CFPB) Consumer Complaint Database** and applies exploratory data analysis, data preprocessing, machine learning classification, model evaluation, threshold tuning, and Principal Component Analysis (PCA).

---

## Table of Contents

- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Project Workflow](#project-workflow)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Preprocessing](#data-preprocessing)
- [Machine Learning Models](#machine-learning-models)
- [Model Evaluation](#model-evaluation)
- [Threshold Tuning](#threshold-tuning)
- [Principal Component Analysis](#principal-component-analysis)
- [Key Findings](#key-findings)
- [Project Structure](#project-structure)
- [Installation and Execution](#installation-and-execution)
- [Limitations](#limitations)
- [Future Scope](#future-scope)
- [References](#references)

---

## Project Overview

Financial consumer complaints provide useful information about problems experienced by customers and how financial companies respond to them.

FinGuard analyzes consumer complaint records to understand:

- Which financial products and services receive complaints.
- What issues are reported most frequently.
- Which companies receive the highest number of complaints.
- How complaints vary across states and submission methods.
- How companies respond to consumer complaints.
- Whether a company's response is classified as timely or untimely.

The main machine learning objective is to predict the **Timely response?** field using classification algorithms.

---

## Objectives

1. Analyze financial consumer complaint data to identify important patterns and trends.
2. Perform exploratory data analysis using statistical summaries and visualizations.
3. Understand the distribution of complaints across products, issues, companies, states, and submission methods.
4. Clean and preprocess the dataset for machine learning.
5. Build and evaluate multiple classification models.
6. Address class imbalance in the target variable.
7. Compare machine learning models using accuracy, precision, recall, and F1-score.
8. Apply threshold tuning to improve the identification of untimely company responses.
9. Apply PCA to reduce feature dimensionality while retaining important information.

---

## Dataset

**Source:** Consumer Financial Protection Bureau (CFPB)

Official dataset: https://www.consumerfinance.gov/data-research/consumer-complaints/

The dataset contains consumer complaint records collected by the CFPB.

### Dataset Details

| Attribute | Details |
|---|---|
| Dataset | CFPB Consumer Complaint Database |
| Time Period | January 2024 – December 2025 |
| Total Records | 95,623 |
| Total Columns | 15 |
| Unique Companies | 517 |
| Target Variable | Timely response? |
| Problem Type | Binary Classification |

### Important Features

| Feature | Description |
|---|---|
| Date received | Date when the complaint was received |
| Product | Financial product associated with the complaint |
| Sub-product | Specific financial service category |
| Issue | Main problem reported by the consumer |
| Company | Financial company associated with the complaint |
| State | Consumer's state |
| Submitted via | Method used to submit the complaint |
| Date sent to company | Date the complaint was forwarded |
| Company response to consumer | Company's response category |
| Timely response? | Indicates whether the response was timely |

The original dataset contains 15 columns. Additional date-based features were created during preprocessing.

**
