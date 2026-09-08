# Supply Chain Delivery Performance Analysis

An end-to-end supply chain analytics project focused on understanding delivery performance, identifying operational bottlenecks, measuring the financial impact of delays, and predicting late-delivery risk using machine learning.

## 📌 Project Overview

Late deliveries can negatively affect customer experience, operational efficiency, and order profitability.

In this project, I analyzed historical supply chain data to understand where delivery delays occur, what operational factors are associated with them, how delays relate to profitability, and whether machine learning can help identify orders at risk of late delivery.

The analysis covers **172,765 orders** from **January 2015 to January 2018**.

## 🎯 Business Objectives

I focused on answering the following business questions:

- How severe is the late-delivery problem?
- Which shipping modes and regions experience the highest delay rates?
- What operational factors are associated with late deliveries?
- How do delivery delays relate to order profitability?
- Are there identifiable time-based patterns in delivery performance?
- Can I predict orders that are at higher risk of late delivery?
- What actions could help improve delivery performance?

## 📊 Executive Summary

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

More than half of the analyzed orders were delivered late, highlighting a significant delivery-performance challenge across the supply chain.

## 🔍 Analysis Performed

### 1. Delivery Performance Analysis

I evaluated delivery performance across multiple operational dimensions, including:

- Shipping mode
- Region
- Customer segment
- Department
- Time period

This helped identify areas with consistently higher delivery-delay rates.

### 2. Profitability Analysis

I examined order profitability and its relationship with delivery delays to understand the financial impact associated with delayed orders.

The analysis found approximately **$2.1M in profit associated with delayed orders**, compared with **$7.5M in total profit** across the analyzed orders.

### 3. Bottleneck Detection

I compared delivery-delay rates across operational categories to identify potential bottlenecks.

Shipping mode showed particularly strong differences in delivery performance, making it an important area for operational investigation.

### 4. Root Cause Analysis

I drilled down into high-delay regions and examined combinations of operational factors such as shipping mode and payment-related conditions.

This analysis helped move from simply identifying *where* delays occur toward understanding *which operational combinations may be contributing to them*.

### 5. Time-Based Analysis

I analyzed delivery delays across:

- Month
- Day of week
- Hour of day

This helped identify periods where delivery performance was comparatively weaker and could support future operational monitoring.

## 🤖 Predictive Modeling

I built a **Random Forest classification model** to predict whether an order was likely to be delivered late.

The modeling workflow included:

- Feature preparation
- Frequency encoding of categorical variables
- Stratified train-test split
- SMOTE for handling class imbalance
- Random Forest classification
- Evaluation using precision, recall, F1-score, and accuracy

### Model Performance

| Metric | Result |
|---|---:|
| Overall Accuracy | 74% |
| Precision for Late Orders | 0.78 |
| Recall for Late Orders | 0.75 |
| F1-Score for Late Orders | 0.77 |

The model identified **75% of actual late orders** in the test set, demonstrating the potential for predictive risk scoring to support proactive delivery interventions.

## 💡 Key Business Insights

- **54.71% of analyzed orders were delivered late**, indicating a substantial delivery-performance issue.
- Delivery performance varied significantly across shipping modes.
- Certain regions showed consistently higher delay rates than others.
- Delivery delays were associated with a measurable amount of order-level profit.
- Customer segment showed relatively limited variation in delay rates compared with operational factors.
- Time-based analysis revealed periods with comparatively higher delay rates.
- The predictive model demonstrated that late-delivery risk can be identified before an order becomes late.

## 🎯 Business Recommendations

Based on the analysis, I recommend:

1. **Prioritize high-risk orders** using predictive risk scores for proactive intervention.
2. **Review underperforming shipping modes** to identify capacity, process, or scheduling issues.
3. **Investigate high-delay regions** and the operational conditions contributing to their performance.
4. **Monitor delivery KPIs continuously** to detect emerging bottlenecks.
5. **Use predictive analytics alongside operational monitoring** to shift from reactive problem-solving toward proactive delivery management.

## 🛠️ Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Imbalanced-learn**
- **Jupyter Notebook**

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
```

## 📄 Project Report

A detailed report containing the complete analysis, findings, predictive modeling results, and recommendations is available in the `reports` folder.

**[View the Detailed Supply Chain Performance Report](Supply_Chain_Performance_Report.pdf)**

## 📓 Notebook

The complete analysis and modeling workflow is available in:

`Supply Chain_Analysis.ipynb`

The notebook covers data preparation, exploratory analysis, KPI development, bottleneck analysis, root-cause analysis, time-based analysis, and predictive modeling.

## 📦 Dataset

The original **DataCo Supply Chain Dataset** is not included in this repository because of its file size.

A `data/README.md` file is provided instead. The notebook contains the data-loading and preprocessing workflow required to reproduce the analysis when the dataset is available locally.

## ⚠️ Limitations

- The analysis is based on historical supply chain data and reflects the patterns present in that dataset.
- The predictive model provides a risk classification rather than a guaranteed outcome.
- The model should be further validated with new operational data before being considered for real-world deployment.
- Additional operational variables could potentially improve predictive performance.

## 🚀 Skills Demonstrated

- Data Cleaning & Preprocessing
- Exploratory Data Analysis
- KPI Development
- Business Performance Analysis
- Bottleneck Detection
- Root Cause Analysis
- Feature Engineering
- Predictive Modeling
- Class Imbalance Handling
- Model Evaluation
- Business Recommendations
- Data Storytelling
