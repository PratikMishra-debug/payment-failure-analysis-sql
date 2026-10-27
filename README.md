# 💳 Payment Failure Analysis — SQL Analytics Case Study

> **A self-directed Data Analytics case study using SQL to analyse payment failures, retry behaviour, failure patterns and potential opportunities for improving payment retry strategies.**

---

## 📌 Project Overview

This project focuses on analysing **payment transaction failures** and understanding how different failure types contribute to retry activity.

The objective is to use SQL-based analysis to identify important failure patterns and translate those findings into potential business recommendations.

The analysis follows:

**Business Problem → Data Analysis → SQL Investigation → Pattern Identification → Recommendation**

---

## 🎯 Business Problem

Payment failures can result in repeated retry attempts, additional processing activity and a poor customer payment experience.

A key question explored in this project is:

> **Which payment failures are associated with repeated retries, and how could retry behaviour be made more efficient?**

The analysis investigates failure codes, retry behaviour and transaction patterns to identify areas where a more targeted retry strategy could be considered.

---

## 📊 Dataset

The project uses a **simulated payment transaction dataset containing approximately 310,000 records**.

The dataset is designed to represent payment activity and includes information relevant to:

- Transactions
- Payment status
- Failure codes
- Retry attempts
- Payment methods
- Transaction characteristics
- Other analytical attributes

> **The dataset is simulated and is not derived from a real production payment system.**

---

## 🛠️ Tools & Technologies

| Category | Technology |
|---|---|
| Database | MySQL |
| Query Language | SQL |
| Analysis | SQL / Excel |
| Data Processing | CTEs |
| Advanced SQL | Window Functions |
| Visualization | Optional / Supporting Analysis |

---

## 🔍 Analysis Performed

### 1. Payment Failure Analysis

Analysed transaction failures to understand:

- Failure frequency
- Failure-code distribution
- Failed transaction patterns
- Contribution of individual failure categories

---

### 2. Retry Behaviour Analysis

Investigated:

- Number of retry attempts
- Retry frequency by failure type
- Failure codes associated with repeated retries
- Distribution of retry activity

---

### 3. Failure-Code Contribution

The analysis identified the failure categories contributing most significantly to retry activity.

In the simulated dataset, **three failure codes accounted for approximately 61% of retry attempts**.

This helped identify failure categories that could be prioritised when evaluating retry policies.

---

### 4. Retry Strategy Analysis

A proposed retry classification/rule was evaluated against the simulated dataset.

The simulated analysis indicated an **estimated 38% reduction in retry volume** under the proposed approach.

> This is a **simulated estimate**, not a measured production outcome.

---

## 🧠 SQL Concepts Used

This project demonstrates practical SQL concepts including:

- `SELECT`
- `WHERE`
- `GROUP BY`
- `HAVING`
- `ORDER BY`
- `CASE`
- Aggregate Functions
- Subqueries
- Common Table Expressions (CTEs)
- Window Functions
- Ranking
- Conditional Analysis
- Data Filtering
- Business KPI Analysis

---

## 🔄 Analytical Workflow

```text
              SIMULATED TRANSACTION DATA
                         │
                         ▼
                   DATA VALIDATION
                         │
                         ▼
                 PAYMENT FAILURES
                    IDENTIFICATION
                         │
                         ▼
                 FAILURE CODE ANALYSIS
                         │
                         ▼
                  RETRY ANALYSIS
                         │
                         ▼
               PATTERN IDENTIFICATION
                         │
                         ▼
                 RETRY RULE ANALYSIS
                         │
                         ▼
              BUSINESS RECOMMENDATION
```

---

## 💡 Key Findings

### Finding 1 — Concentrated Retry Activity

In the simulated dataset:

> **Three failure codes accounted for approximately 61% of retry attempts.**

This suggests that retry behaviour is not evenly distributed across all failure categories.

---

### Finding 2 — Targeted Retry Strategy

The analysis explored a proposed approach where retry behaviour is differentiated according to failure characteristics rather than applying the same retry behaviour to every failure.

---

### Finding 3 — Simulated Impact

Under the proposed rule applied to the simulated dataset:

> **Estimated retry volume reduction: 38%**

This result should be interpreted as a **scenario-based estimate**, not a production KPI.

---

## 💼 Business Recommendation

Based on the analysis, a payment platform could consider:

- Classifying failures according to their likelihood of recovery
- Applying retry logic selectively
- Avoiding unnecessary retries for non-recoverable failures
- Monitoring retry behaviour by failure category
- Continuously evaluating retry success rates
- Testing proposed rules against historical production data before implementation

---

## 📈 Potential Business Metrics

A production implementation could monitor:

- Payment Success Rate
- Payment Failure Rate
- Retry Rate
- Retry Success Rate
- Failure-Code Distribution
- Average Retry Attempts
- Unnecessary Retry Rate
- Transaction Recovery Rate

---

## 📁 Project Structure

```text
payment-failure-analysis-sql/
│
├── README.md
│
├── data/
│   └── simulated_transactions.csv
│
├── sql/
│   ├── 01_data_validation.sql
│   ├── 02_failure_analysis.sql
│   ├── 03_retry_analysis.sql
│   ├── 04_failure_code_analysis.sql
│   └── 05_retry_strategy.sql
│
├── documentation/
│   └── payment_failure_analysis.pdf
│
└── screenshots/
    └── ...
```

---

## ⚠️ Project Disclaimer

> **This is a self-directed portfolio case study created for educational and demonstration purposes. The dataset and business scenario are simulated and are not based on confidential client information or a live payment-processing environment.**

> The reported percentages and estimated impact represent calculations or scenario-based results from the simulated dataset and should not be interpreted as real-world production outcomes.

---

## 🧠 What This Project Demonstrates

This project demonstrates my ability to:

- Translate a business problem into analytical questions
- Work with a large simulated transaction dataset
- Write SQL queries for business analysis
- Analyse payment failures and retry behaviour
- Use CTEs and window functions
- Identify meaningful patterns in transactional data
- Convert analytical findings into business recommendations
- Communicate limitations and assumptions clearly

---

## 👨‍💻 Author

**Pratik Kumar**

B.Tech — Computer Science & Information Technology

**Career Focus:** Business Analysis | Data Analytics | Business Intelligence | Technology & Consulting

---

⭐ Explore my other projects for Business Analysis and Power BI case studies.
