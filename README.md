# Supply Chain Delivery Performance Analysis

An end-to-end analysis of supply chain delivery performance focused on identifying operational bottlenecks, understanding the financial impact of delivery delays, and predicting orders at risk of late delivery.

## 📌 Business Problem

Late deliveries can affect customer satisfaction, operational efficiency, and order profitability.

In this project, I analyzed historical supply chain data to answer three key questions:

- Where are delivery delays occurring most frequently?
- What operational factors are associated with late deliveries?
- Can I identify orders that are at higher risk of being delivered late?

## 📊 Executive Summary

I analyzed 172,765 orders covering the period from January 2015 to January 2018.

| KPI | Result |
|---|---:|
| Total Orders Analyzed | 172,765 |
| Late Deliveries | 94,523 |
| Late Delivery Rate | 54.71% |
| On-Time Delivery Rate | 45.29% |
| Total Profit | $7.5M |
| Profit Associated with Delayed Orders | $2.1M |
| 90th Percentile Delay | 3 days |
| Average Order Profit | $22.03 |

The analysis showed that late delivery is a significant operational issue, with more than half of analyzed orders delivered late. Supply_Chain_Performance_Report(1).pdf

## 🔍 What I Analyzed

### 1. Delivery Performance
I evaluated delivery performance across:

- Shipping modes
- Regions
- Customer segments
- Departments
- Time periods

### 2. Profitability Impact

I examined the relationship between delivery delays and order profitability to understand the financial impact associated with delayed orders.

### 3. Bottleneck Detection

I compared delay rates across operational dimensions to identify areas with consistently higher delivery risk.

### 4. Root Cause Analysis

I drilled into high-delay regions and examined shipping modes and operational factors to identify potential contributors to delivery problems.

### 5. Time-Based Patterns

I analyzed delivery performance by:

- Month
- Day of week
- Hour of day

### 6. Predictive Modeling

I built a Random Forest classification model to predict whether an order was likely to be delivered late.

The modeling workflow included:

- Categorical feature encoding
- Stratified train-test split
- SMOTE for class imbalance
- Random Forest classification

## 🤖 Model Performance

The model achieved:

| Metric | Result |
|---|---:|
| Accuracy | 74% |
| Precision for Late Orders | 0.78 |
| Recall for Late Orders | 0.75 |
| F1-Score for Late Orders | 0.77 |

The model correctly identified 75% of actual late orders in the test set, providing a useful starting point for risk-based intervention. Supply_Chain_Performance_Report(1).pdf

## 💡 Key Business Insights

- More than half of analyzed orders were delivered late.
- Delivery performance varied considerably across shipping modes.
- Certain regions and operational combinations showed substantially higher delay rates.
- Delivery delays were associated with a measurable amount of order-level profit.
- Customer segment alone did not appear to be a major differentiator in delivery performance.
- The predictive model demonstrated that late-delivery risk can be identified before an order becomes late.

## 🎯 Recommendations

Based on the analysis, I would recommend:

1. Prioritizing high-risk orders for proactive intervention.
2. Reviewing consistently underperforming shipping modes and regions.
3. Investigating operational bottlenecks in high-delay areas.
4. Using predictive risk scores to support fulfillment and logistics decisions.
5. Continuously monitoring delivery KPIs to identify emerging performance issues.

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- Jupyter Notebook

## 📁 Repository Structure

```text
supply-chain-delivery-performance-analysis/
│
├── README.md
│
├── data/
│   └── README.md
│
├── notebooks/
│   └── supply_chain_analysis.ipynb
│
├── reports/
│   └── supply_chain_delivery_performance_report.pdf
│
├── images/
│   ├── executive-summary.png
│   ├── bottleneck-analysis.png
│   ├── root-cause-analysis.png
│   └── model-performance.png
│
├── requirements.txt
│
└── .gitignore# Supply Chain Delivery Performance Analysis

An end-to-end analysis of supply chain delivery performance focused on identifying operational bottlenecks, understanding the financial impact of delivery delays, and predicting orders at risk of late delivery.

## 📌 Business Problem

Late deliveries can affect customer satisfaction, operational efficiency, and order profitability.

In this project, I analyzed historical supply chain data to answer three key questions:

- Where are delivery delays occurring most frequently?
- What operational factors are associated with late deliveries?
- Can I identify orders that are at higher risk of being delivered late?

## 📊 Executive Summary

I analyzed 172,765 orders covering the period from January 2015 to January 2018.

| KPI | Result |
|---|---:|
| Total Orders Analyzed | 172,765 |
| Late Deliveries | 94,523 |
| Late Delivery Rate | 54.71% |
| On-Time Delivery Rate | 45.29% |
| Total Profit | $7.5M |
| Profit Associated with Delayed Orders | $2.1M |
| 90th Percentile Delay | 3 days |
| Average Order Profit | $22.03 |

The analysis showed that late delivery is a significant operational issue, with more than half of analyzed orders delivered late. Supply_Chain_Performance_Report(1).pdf

## 🔍 What I Analyzed

### 1. Delivery Performance
I evaluated delivery performance across:

- Shipping modes
- Regions
- Customer segments
- Departments
- Time periods

### 2. Profitability Impact

I examined the relationship between delivery delays and order profitability to understand the financial impact associated with delayed orders.

### 3. Bottleneck Detection

I compared delay rates across operational dimensions to identify areas with consistently higher delivery risk.

### 4. Root Cause Analysis

I drilled into high-delay regions and examined shipping modes and operational factors to identify potential contributors to delivery problems.

### 5. Time-Based Patterns

I analyzed delivery performance by:

- Month
- Day of week
- Hour of day

### 6. Predictive Modeling

I built a Random Forest classification model to predict whether an order was likely to be delivered late.

The modeling workflow included:

- Categorical feature encoding
- Stratified train-test split
- SMOTE for class imbalance
- Random Forest classification

## 🤖 Model Performance

The model achieved:

| Metric | Result |
|---|---:|
| Accuracy | 74% |
| Precision for Late Orders | 0.78 |
| Recall for Late Orders | 0.75 |
| F1-Score for Late Orders | 0.77 |

The model correctly identified 75% of actual late orders in the test set, providing a useful starting point for risk-based intervention. Supply_Chain_Performance_Report(1).pdf

## 💡 Key Business Insights

- More than half of analyzed orders were delivered late.
- Delivery performance varied considerably across shipping modes.
- Certain regions and operational combinations showed substantially higher delay rates.
- Delivery delays were associated with a measurable amount of order-level profit.
- Customer segment alone did not appear to be a major differentiator in delivery performance.
- The predictive model demonstrated that late-delivery risk can be identified before an order becomes late.

## 🎯 Recommendations

Based on the analysis, I would recommend:

1. Prioritizing high-risk orders for proactive intervention.
2. Reviewing consistently underperforming shipping modes and regions.
3. Investigating operational bottlenecks in high-delay areas.
4. Using predictive risk scores to support fulfillment and logistics decisions.
5. Continuously monitoring delivery KPIs to identify emerging performance issues.

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- Jupyter Notebook

## 📁 Repository Structure

```text
supply-chain-delivery-performance-analysis/
│
├── README.md
│
├── data/
│   └── README.md
│
├── notebooks/
│   └── supply_chain_analysis.ipynb
│
├── reports/
│   └── supply_chain_delivery_performance_report.pdf
│
├── images/
│   ├── executive-summary.png
│   ├── bottleneck-analysis.png
│   ├── root-cause-analysis.png
│   └── model-performance.png
│
├── requirements.txt
│
└── .gitignore
