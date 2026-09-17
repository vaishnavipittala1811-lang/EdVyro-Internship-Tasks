# 📊 Customer Intelligence 360

### End-to-End Customer Churn & Retention Analytics Project

> **Internship Analytics Capstone Project**
> Data Quality → Exploratory Data Analysis → Business KPIs → Customer Segmentation → Risk Analysis → Retention Strategy

---

## 📌 Project Overview

**Customer Intelligence 360** is an end-to-end customer analytics project developed as part of an internship program.

The project analyzes customer behavior, identifies the major factors associated with customer churn, segments customers based on their characteristics, evaluates customer risk, and converts the analysis into actionable retention strategies.

Instead of treating each internship task as a separate analysis, this project combines the complete workflow into one integrated analytics solution.

### 🎯 Core Business Question

> **Who is likely to churn, why are they at risk, how valuable are they, and what action should the business take?**

The project follows the complete analytics journey:

```text
Raw Customer Data
       ↓
Data Quality & Cleaning
       ↓
Exploratory Data Analysis
       ↓
Business KPI Analysis
       ↓
Churn Driver Analysis
       ↓
Customer Segmentation
       ↓
Customer Risk Scoring
       ↓
Revenue-at-Risk Analysis
       ↓
Retention Recommendations
       ↓
Executive Analytics Dashboard
```

---

# 🏢 Internship Tasks Covered

This repository combines the following internship tasks:

| Task        | Focus Area                    | Key Outcome                                             |
| ----------- | ----------------------------- | ------------------------------------------------------- |
| **Task 02** | Data Quality & EDA            | Understand and validate customer data                   |
| **Task 03** | Business KPI Dashboard        | Measure churn, retention and revenue exposure           |
| **Task 04** | Segmentation & Recommendation | Identify customer segments and risk levels              |
| **Task 05** | Executive Analytics Capstone  | Combine all insights into one decision-support solution |

---

# 🎯 Project Objectives

The main objectives of this project are:

* Perform data quality assessment and cleaning.
* Explore customer demographics and service characteristics.
* Analyze customer churn patterns.
* Calculate important business KPIs.
* Identify major churn drivers.
* Segment customers using clustering techniques.
* Develop an explainable customer risk score.
* Identify high-value customers at risk.
* Estimate monthly revenue exposed to churn.
* Prioritize customers for retention campaigns.
* Generate personalized retention recommendations.
* Perform retention scenario analysis.
* Build an executive-level analytical view.
* Convert analytical findings into business decisions.

---

# 📂 Dataset

The project uses a customer churn dataset containing information about customers, their subscription details, usage characteristics, charges, support interactions and churn status.

### Important Features

| Feature            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `CustomerID`       | Unique customer identifier                              |
| `Age`              | Customer age                                            |
| `TenureMonths`     | Number of months the customer has been with the company |
| `MonthlyCharges`   | Recurring monthly customer charge                       |
| `TotalCharges`     | Total customer charges                                  |
| `SupportTickets`   | Number of support tickets raised                        |
| `Contract`         | Customer contract type                                  |
| `PaymentMethod`    | Customer payment method                                 |
| `SubscriptionType` | Customer subscription category                          |
| `Churn`            | Whether the customer has churned                        |

Additional analytical columns were created during the project, including:

* `TenureGroup`
* `SegmentName`
* `RiskScore`
* `RiskCategory`
* `RiskFactors`
* `Recommendation`
* `PriorityScore`
* `PriorityRank`

---

# 🛠️ Technologies & Tools

The project was primarily developed using **Google Colab** and Python.

### Programming Language

* Python

### Libraries

* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical computation
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine learning and customer segmentation
* **IPyWidgets** – Optional interactive analysis

### Development Environment

* Google Colab
* Jupyter Notebook

---

# 🔎 Task 02 — Data Quality & Exploratory Analysis

The first stage focuses on understanding the quality and structure of the dataset.

## Data Quality Checks

The following checks were performed:

* Dataset dimensions
* Column names
* Data types
* Missing values
* Duplicate rows
* Duplicate Customer IDs
* Unique categorical values
* Descriptive statistics
* Numerical outlier detection
* Data consistency validation

## Exploratory Analysis

The project explores:

* Customer age distribution
* Customer tenure
* Monthly charges
* Total charges
* Support ticket behavior
* Contract types
* Payment methods
* Subscription types
* Churn distribution

### Key Visualizations

* Histograms
* Box plots
* Bar charts
* Churn distribution charts
* Correlation heatmap
* Churn-by-category charts

---

# 📈 Task 03 — Business KPI Dashboard

The second stage transforms the dataset into meaningful business metrics.

## Key Performance Indicators

The project calculates:

### 👥 Total Customers

Total number of customers in the dataset.

### 🚨 Churned Customers

Number of customers who have left the service.

### 📉 Churn Rate

```text
Churn Rate =
Churned Customers / Total Customers × 100
```

### 💚 Retention Rate

```text
Retention Rate =
Retained Customers / Total Customers × 100
```

### 💰 Total Monthly Revenue

Sum of the monthly charges of all active customers represented in the dataset.

### ⚠️ Monthly Revenue at Risk

Monthly recurring charges associated with churned customers.

```text
Revenue at Risk =
Sum of MonthlyCharges for Churned Customers
```

### 💡 Revenue-at-Risk Percentage

```text
Revenue-at-Risk % =
Revenue at Risk / Total Monthly Revenue × 100
```

> **Note:** `MonthlyCharges` represents recurring revenue exposure. `TotalCharges` is historical customer value and should not be interpreted as recurring revenue at risk.

---

# 👥 Task 04 — Customer Segmentation & Recommendation Model

The third stage applies analytical and machine-learning techniques to understand different types of customers.

## Customer Segmentation

K-Means clustering is used to group customers based on numerical characteristics such as:

* Age
* Tenure
* Monthly Charges
* Support Tickets

Before clustering, numerical features are standardized using `StandardScaler`.

### Example Segmentation Concept

Customers may be grouped into profiles such as:

* New / Emerging Customers
* Loyal Customers
* High-Value Customers
* High-Support Customers
* At-Risk Customers

The exact segment names are generated based on the resulting cluster profiles.

---

# ⚠️ Customer Risk Scoring

An explainable risk-scoring framework is used to identify customers who may require retention attention.

Potential risk signals include:

* Short customer tenure
* Month-to-month contracts
* Higher support ticket volume
* Specific payment methods
* Certain subscription types
* Existing churn status

Customers are classified into categories such as:

```text
Low Risk
Medium Risk
High Risk
```

The objective is not simply to assign a score, but to explain **why** a customer is considered risky.

---

# 🎯 Retention Recommendations

Each customer can receive a recommendation based on their risk profile and customer characteristics.

Examples include:

* Contract upgrade offers
* Loyalty benefits
* Customer support follow-up
* Payment-method assistance
* Personalized discounts
* Subscription upgrades
* Proactive engagement campaigns

This transforms the project from descriptive analytics into **prescriptive business analytics**.

---

# 🚀 Task 05 — Customer Intelligence 360

Task 05 combines the previous tasks into a single executive analytics solution.

Instead of presenting four disconnected assignments, the final capstone answers four important questions:

```text
WHO?
Which customers are at risk?

WHY?
What factors are associated with their risk?

VALUE?
How much recurring revenue is exposed?

ACTION?
What should the business do next?
```

---

# 📊 Advanced Visualizations

The capstone includes additional visualizations to improve understanding of the dataset.

### 1. Customer Profile Distribution

Shows the overall distribution of important numerical customer attributes.

### 2. Customer Value vs Tenure

Analyzes the relationship between:

* Customer tenure
* Monthly charges

This helps identify valuable long-term and potentially valuable new customers.

### 3. Monthly Charges vs Support Tickets

Helps understand whether high-value customers also require more support.

### 4. Customer Retention Overview

Provides a visual comparison between:

* Retained customers
* Churned customers

### 5. Churn Driver Analysis

Compares churn behavior across:

* Contract types
* Payment methods
* Subscription types
* Tenure groups
* Support-ticket groups

### 6. Revenue Exposure Matrix

Combines customer risk with monthly charges to identify financially important customers.

### 7. Risk Score vs Customer Value

Visualizes customers based on:

```text
Risk Score
        ×
Monthly Charges
```

This helps prioritize retention actions.

### 8. Customer Journey Risk Map

Analyzes customer risk across different tenure stages.

### 9. Retention Opportunity Ranking

Ranks customers according to their retention priority.

### 10. Executive Dashboard

Combines the most important KPIs and analytical findings into one final view.

---

# 💰 Retention What-If Analysis

One of the additional features introduced in the capstone is a **Retention What-If Simulator**.

The analysis estimates how much monthly revenue could potentially be preserved if a certain percentage of high-risk churned customers were successfully retained.

Example scenarios:

| Retention Scenario | Potential Revenue Preserved               |
| ------------------ | ----------------------------------------- |
| 25%                | Calculated from high-risk churned revenue |
| 50%                | Calculated from high-risk churned revenue |
| 75%                | Calculated from high-risk churned revenue |
| 100%               | Maximum scenario                          |

### Important

This is a **scenario analysis**, not a financial forecast.

It demonstrates the potential business impact of retention rather than predicting actual future revenue.

---

# 💡 Retention Priority Score

A custom analytical priority score is created using:

```text
PriorityScore =
RiskScore × MonthlyCharges
```

This allows customers to be prioritized based on both:

* Probability/level of risk
* Financial importance

Customers with high risk and high monthly charges receive greater retention priority.

> The Priority Score is an analytical prioritization metric and should not be interpreted as a machine-learning probability of churn.

---

# 🚨 Executive Action Matrix

The final project converts analytics into business actions.

| Customer Situation           | Recommended Action                            |
| ---------------------------- | --------------------------------------------- |
| 🔴 High Risk + High Charges  | Immediate personalized retention intervention |
| 🔴 High Risk + Lower Charges | Targeted retention campaign                   |
| 🟠 Medium Risk               | Proactive engagement and monitoring           |
| 🟢 Low Risk                  | Maintain regular engagement                   |
| 🟢 Low Risk + High Value     | Loyalty and relationship-building initiatives |

---

# 📌 Key Analytical Findings

The dataset analysis revealed several strong patterns in the sample.

### Contract Type

Month-to-month customers showed substantially higher churn than customers on longer contracts.

### Tenure

Customers with shorter tenure demonstrated considerably higher churn in the sample.

### Support Tickets

Customers with more support tickets showed a strong association with churn.

### Subscription Type

Some subscription categories showed higher churn levels than others.

### Payment Method

Certain payment methods showed higher churn rates in the sample.

### Revenue Exposure

Customers who combine:

```text
High Risk
+
High Monthly Charges
```

represent the most important retention opportunities.

> Because this dataset is very small and synthetic, these patterns should be treated as **descriptive findings from the sample**, not as statistically generalizable conclusions about a larger customer population.

---

# 🧠 Business Insights

The project demonstrates that customer churn should not be analyzed using churn status alone.

A better approach is to combine:

```text
Customer Behaviour
        +
Customer Value
        +
Customer Risk
        +
Customer Segment
        =
Retention Priority
```

For example, two customers may both be classified as high risk, but the customer with significantly higher monthly charges may deserve more immediate intervention.

This creates a more practical business-oriented retention strategy.

---

# 📋 Final Business Recommendations

Based on the analysis, businesses could consider:

### 1. Strengthen Early Customer Engagement

Customers in the first few months should receive proactive onboarding and engagement.

### 2. Encourage Longer Contracts

Month-to-month customers can be targeted with incentives for longer-term contracts.

### 3. Improve Support Experience

Customers with repeated support tickets should receive proactive service recovery.

### 4. Protect High-Value Customers

High-risk customers with high monthly charges should receive personalized retention attention.

### 5. Monitor Payment Experience

Payment-method-related friction should be investigated where higher churn is observed.

### 6. Use Customer Segmentation

Different customer groups should receive different retention strategies instead of using one campaign for everyone.

### 7. Prioritize Based on Business Value

Retention resources should focus first on customers who combine high risk with high recurring revenue exposure.

---

# 📁 Recommended Repository Structure

```text
Customer-Intelligence-360/
│
├── README.md
│
├── data/
│   ├── customer_churn_sample.csv
│   └── customer_churn_cleaned.csv
│
├── notebooks/
│   └── Customer_Intelligence_360.ipynb
│
├── outputs/
│   └── customer_churn_task04_results.csv
│
└── screenshots/
    ├── data_quality.png
    ├── kpi_dashboard.png
    ├── churn_analysis.png
    ├── segmentation.png
    ├── risk_analysis.png
    └── executive_dashboard.png
```

---

# ▶️ How to Run the Project

## Option 1 — Google Colab

1. Open the project notebook in Google Colab.
2. Upload the customer churn CSV dataset.
3. Run the notebook cells sequentially.
4. Review the data-quality analysis.
5. Explore the visualizations.
6. Review the KPI dashboard.
7. Run customer segmentation.
8. Review risk scores and recommendations.
9. Explore the executive analytics section.
10. Download the generated results if required.

---

# 📦 Installation

If running outside Google Colab, install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

For optional interactive widgets:

```bash
pip install ipywidgets
```

---

# 🔬 Analytical Methodology

The project follows this methodology:

### Step 1 — Data Understanding

Understand dataset structure, variables and business context.

### Step 2 — Data Quality

Check:

* Missing values
* Duplicates
* Data types
* Invalid values
* Outliers
* Customer ID uniqueness
* Charge consistency

### Step 3 — Exploratory Data Analysis

Analyze customer behavior using descriptive statistics and visualizations.

### Step 4 — KPI Development

Convert raw customer information into business metrics.

### Step 5 — Churn Driver Analysis

Identify characteristics associated with customer churn.

### Step 6 — Customer Segmentation

Apply K-Means clustering to identify customer groups.

### Step 7 — Risk Analysis

Calculate explainable customer risk scores.

### Step 8 — Value Analysis

Measure monthly revenue exposure associated with churn-risk customers.

### Step 9 — Retention Prioritization

Combine customer risk and financial value.

### Step 10 — Executive Recommendations

Translate analytical results into actionable business strategies.

---

# 📊 Project Architecture

```text
                    ┌──────────────────────┐
                    │   Customer Dataset   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │   Data Quality       │
                    │   & Cleaning         │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Exploratory Analysis │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              ▼                ▼                ▼
       ┌────────────┐   ┌────────────┐   ┌────────────┐
       │    KPIs    │   │ Churn      │   │ Customer   │
       │            │   │ Drivers    │   │ Segments   │
       └─────┬──────┘   └─────┬──────┘   └─────┬──────┘
             │                │                │
             └────────────────┼────────────────┘
                              ▼
                    ┌──────────────────────┐
                    │   Risk Scoring       │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Revenue Exposure     │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Retention Priority   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Executive Insights   │
                    │ & Recommendations    │
                    └──────────────────────┘
```

---

# 📈 Skills Demonstrated

This internship project demonstrates practical skills in:

### 🐍 Python

* Data manipulation
* Data cleaning
* Conditional logic
* Functions
* Data aggregation

### 📊 Data Analytics

* Exploratory Data Analysis
* Descriptive statistics
* KPI development
* Business analysis
* Customer behavior analysis

### 📉 Data Visualization

* Matplotlib
* Seaborn
* Distribution analysis
* Comparative analysis
* Correlation analysis
* Executive dashboards

### 🤖 Machine Learning

* Feature selection
* Feature scaling
* K-Means clustering
* Customer segmentation

### 🧠 Business Intelligence

* Churn analysis
* Revenue-at-risk analysis
* Customer prioritization
* Retention strategy
* Scenario analysis

### 💼 Business Communication

* Executive insights
* Data storytelling
* Action-oriented recommendations
* Decision-support analytics

---

# 🌟 What Makes This Project Different?

Most basic churn projects stop at:

```text
"Which customers churned?"
```

This project goes further:

```text
Which customers churned?
             ↓
What characteristics are associated with churn?
             ↓
Which customers belong to similar segments?
             ↓
Who is currently at risk?
             ↓
Which risky customers are financially important?
             ↓
How much recurring revenue is exposed?
             ↓
Who should the business contact first?
             ↓
What retention strategy should be used?
```

Therefore, the project moves from **descriptive analytics** toward **prescriptive decision support**.

---

# ⚠️ Project Limitations

The dataset used for this internship project is small and synthetic.

Therefore:

* Churn percentages are sample-specific.
* Segment patterns may change with a larger dataset.
* Risk scoring is an analytical framework rather than a validated predictive model.
* The retention what-if analysis is scenario analysis, not a forecast.
* Correlation does not imply causation.
* Business decisions should be validated using larger real-world datasets.

For production use, the solution should be tested on a much larger historical dataset and evaluated using appropriate machine-learning validation techniques.

---

# 🔮 Future Improvements

The project can be extended into a production-level customer intelligence system by adding:

### Machine Learning Churn Prediction

Implement models such as:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost
* Gradient Boosting

### Model Evaluation

Add:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC
* Confusion Matrix

### Explainable AI

Use:

* SHAP
* Feature importance
* Individual customer explanations

### Real-Time Analytics

Connect the model to:

* CRM systems
* Customer support platforms
* Transaction databases

### Advanced Dashboard

Build a production dashboard using:

* Power BI
* Tableau
* Looker Studio
* Streamlit

### Automated Retention System

Automatically trigger:

```text
High Risk Customer
        ↓
Identify Risk Factor
        ↓
Select Retention Strategy
        ↓
Send Personalized Offer
        ↓
Track Customer Response
```

---

# 🏆 Final Outcome

The final internship project delivers a complete customer analytics workflow capable of:

✅ Cleaning and validating customer data
✅ Exploring customer behavior
✅ Measuring business KPIs
✅ Understanding churn patterns
✅ Segmenting customers
✅ Scoring customer risk
✅ Identifying revenue exposure
✅ Prioritizing retention opportunities
✅ Generating customer recommendations
✅ Performing retention scenario analysis
✅ Presenting executive-level insights

---

# 📌 Final Takeaway

> **Customer Intelligence 360 transforms raw customer data into actionable retention intelligence.**

The project demonstrates how data analytics can move beyond charts and statistics to answer practical business questions.

The final framework is:

```text
DATA
 ↓
INSIGHT
 ↓
RISK
 ↓
VALUE
 ↓
ACTION
```

or, more specifically:

> **WHO is at risk → WHY are they at risk → HOW valuable are they → WHAT should the business do?**

---

## 👨‍💻 Project Type

**Internship Analytics Project / Capstone**

**Domain:** Customer Analytics & Business Intelligence

**Primary Focus:** Customer Churn, Segmentation & Retention

**Environment:** Google Colab / Jupyter Notebook

**Language:** Python

---
