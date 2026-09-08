# Supply Chain Delivery Performance Analysis

An end-to-end supply chain analytics project focused on identifying delivery bottlenecks, quantifying the financial impact of late deliveries, and building a machine learning model to identify orders at risk of late delivery.

![Supply Chain Analysis](images/executive-summary.png)

## 📌 Business Problem

Late deliveries can directly affect customer experience, operational efficiency, and order profitability.

In this project, I analyzed order fulfillment data to answer a central business question:

> **Why are orders being delivered late, where are the major operational bottlenecks, and how can the business improve on-time delivery while protecting profitability?**

The analysis focuses on understanding delivery performance across regions, customer segments, shipping modes, departments, payment types, and order status.

---

## 🎯 Objectives

I structured the analysis around five key objectives:

- Understand the current state of delivery performance.
- Quantify the financial impact of delayed deliveries.
- Identify the operational dimensions associated with higher delay rates.
- Investigate potential root causes behind late deliveries.
- Build a predictive model to identify orders at higher risk of late delivery.

---

## 📊 Dataset

The analysis uses an e-commerce supply chain dataset containing order, customer, product, shipping, payment, and profitability information.

The original dataset contains **180,519 records and 53 columns**.

After data cleaning and filtering, **172,765 orders** were used for the final analysis.

The data covers orders from **January 2015 to January 2018**.

Key variables include:

- Shipping mode
- Actual shipping days
- Scheduled shipping days
- Order date
- Shipping date
- Delivery status
- Late delivery risk
- Customer segment
- Customer region
- Department
- Payment type
- Order status
- Sales
- Order profit
- Product information

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**

### Machine Learning

- Frequency Encoding
- Train/Test Split
- SMOTE
- Random Forest Classifier
- Classification Metrics

---

## 🔄 Project Workflow

```text
Raw Supply Chain Data
        ↓
Data Quality Assessment
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
Business KPI Analysis
        ↓
Bottleneck Detection
        ↓
Root Cause Analysis
        ↓
Time-Based Analysis
        ↓
Predictive Modeling
        ↓
Business Recommendations
