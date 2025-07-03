# 🏦 Bank Customer Churn Analysis – Power BI

A Power BI report analyzing factors affecting customer churn in a banking dataset.

## 🎯 Project Objective

Identify which customer attributes drive churn and visualize trends to help business decision-making.

## 🔧 Tools Used
- Power BI Desktop + Service
- DAX (Power BI measures)

## 🧩 Data Preparation
- Cleaned customer attributes (gender, tenure, products, balance)
- Handled missing values and formatted dates

## 📊 Key Metrics & DAX Measures

`dax
CustomerChurn_rate = DIVIDE(
  COUNTROWS(FILTER(Customers, Customers[Churn] = "Yes")),
  COUNTROWS(Customers),
  0
)

## 🛠️ Key Steps
Data Connection: Loaded CSV bank-churn dataset via Power BI Get Data

Preparation: Cleaned, formatted, and transformed columns (e.g. Binary → Yes/No, Age, Balance)

Modeling: Created relationships and summarized tables

Analysis & DAX: Measures like:

CustomerChurn_rate = DIVIDE(COUNTROWS(FILTER(Customers, Churn = "Yes")), COUNTROWS(Customers))

Visualizations: Churn rate by tenure, geography, products, credit score, balance; combined slicers for segmentation

Themes & Formatting: Applied a modern theme, consistent branding, clean tooltips

Publishing: Report published to Power BI Service and shared via URL

## 📈 Dashboard Overview
Churn Rate by tenure, geography, product count, balance tier, credit score segment

Drill-through functionality and slicer-based filters

KPIs: Total Customers, Total Churned, Churn %, Avg Balance

## 💡 Key Insights
Higher churn among customers with fewer products

Churn peaks for customers with low tenure and low balance

Certain regions and demographics show elevated turnover

## 📈 Insights Highlighted
Churn increases when customers hold few products

Customers with low tenure and low balance tend to churn

Segment-wise churn shows specific regional or demographic risks

## Contact
Nikhil Chavan

Email: nikhilcaptain4@gmail.com

LinkedIn: linkedin.com/in/nikhil-c-993548151
