🧩 Customer Segmentation using RFM Analysis

IE6400 – Foundations of Data Analytics Engineering

📌 Overview

This project applies RFM (Recency, Frequency, Monetary) analysis and K-Means clustering to segment customers based on purchasing behavior using a real-world eCommerce transactions dataset. The goal is to identify high-value customers, understand behavioral patterns, and translate insights into actionable marketing strategies. 

Project2_Report

🎯 Objectives

Compute Recency, Frequency, and Monetary metrics for each customer

Create rule-based RFM segments using quartile scoring

Apply K-Means clustering to automatically discover customer groups

Profile each segment using behavioral and revenue characteristics

Translate analytical insights into business and marketing recommendations

🛠️ Tools & Technologies

Language: Python

Libraries: pandas, NumPy, scikit-learn, matplotlib, seaborn

Techniques: Data Cleaning, Feature Engineering, RFM Analysis, Clustering

Environment: Jupyter Notebook

📂 Dataset

Source: Online Retail eCommerce dataset (Kaggle)

Size (raw): ~541K transaction records

Size (cleaned): ~398K records after removing returns

Time period: December 2010 – December 2011

Key fields: InvoiceDate, CustomerID, Quantity, UnitPrice, Country

🔧 Methodology
1️⃣ Data Preprocessing

Converted invoice dates to datetime and engineered time-based features

Removed returned transactions (negative quantities) for accurate RFM analysis

Created TotalPrice = Quantity × UnitPrice

Filtered valid customers and standardized data types

2️⃣ RFM Metric Computation

Recency: Days since last purchase

Frequency: Number of unique invoices per customer

Monetary: Total revenue per customer

Aggregated metrics for 4,339 unique customers

3️⃣ RFM Scoring

Assigned quartile-based scores (1–4) for R, F, and M

Created combined RFM scores and overall RFM sum for interpretation

4️⃣ Clustering

Standardized RFM variables using StandardScaler

Evaluated K-Means models (k = 2–6) using silhouette scores

Selected k = 2 due to strong cluster separation

Identified:

Cluster 0: Regular / Low–Medium Value Customers

Cluster 1: VIP / Champion Customers

📊 Key Insights

Less than 1% of customers contribute ~25% of total revenue, highlighting the importance of VIP retention

Majority of customers exhibit low-to-moderate engagement and spending

Clear behavioral separation exists between high-value and regular customers

RFM metrics provide interpretable and actionable segmentation for marketing

💡 Business Recommendations

VIP Customers: Loyalty programs, personalized offers, early access incentives

Regular Customers: Re-engagement campaigns, cross-sell and upsell strategies

At-Risk Customers: Win-back campaigns based on recency decline
