 Marketing Funnel & Lead Conversion Performance Dashboard

A professional Power BI dashboard that analyzes marketing funnel performance, lead acquisition, and conversion rates using the Olist Marketing Funnel dataset. The dashboard provides actionable insights into marketing channel effectiveness, landing page performance, and lead conversion trends to support data-driven business decisions.

---

## 📌 Project Overview

Marketing teams invest significant resources in acquiring leads through multiple channels. However, understanding which channels generate high-quality leads and where potential customers drop off in the funnel is critical for improving marketing ROI.

This project uses Power BI to transform raw marketing data into an interactive dashboard that enables stakeholders to monitor lead acquisition, evaluate conversion performance, and identify optimization opportunities.

---

 Business Objectives

The dashboard answers the following business questions:

- How many leads were generated?
- What percentage of leads converted into customers?
- Which marketing channels generate the highest number of leads?
- Which marketing channels have the highest conversion rates?
- Which landing pages perform best?
- How has lead acquisition changed over time?
- How has conversion performance changed over time?

---

## 📂 Dataset

**Dataset:** Olist Marketing Funnel Dataset

Main table used:

- `funnel_cleaned`

Key fields:

- `mql_id`
- `first_contact_date`
- `origin`
- `landing_page_id`
- `converted`

---

## 🛠 Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Excel / CSV
- Git & GitHub

---

## 📈 Dashboard Features

### Executive KPI Cards

- Total Leads
- Converted Leads
- Overall Conversion Rate

### Interactive Visualizations

- Lead Acquisition Trend
- Conversion Rate Trend
- Leads by Marketing Origin
- Conversion Rate by Origin
- Top Performing Landing Pages
- Conversion Status Distribution

### Interactive Filters

- Year
- Quarter
- Marketing Origin

---

## 📊 DAX Measures

### Total Leads

```DAX
Total Leads =
COUNT(funnel_cleaned[mql_id])
```

### Converted Leads

```DAX
Converted Leads =
CALCULATE(
    COUNTROWS(funnel_cleaned),
    funnel_cleaned[converted] = TRUE()
)
```

### Conversion Rate

```DAX
Conversion Rate =
DIVIDE(
    [Converted Leads],
    [Total Leads],
    0
)
```

---

## 📷 Dashboard Preview

> Replace this image after uploading your dashboard screenshot.

![Dashboard Preview](images/dashboard-overview.png)

---

## 📌 Key Insights

The dashboard enables users to:

- Monitor overall marketing performance.
- Identify the most effective lead acquisition channels.
- Compare conversion rates across marketing origins.
- Discover high-performing landing pages.
- Analyze lead generation trends over time.
- Filter results dynamically by year, quarter, and origin.

---

## 💼 Business Value

This dashboard helps marketing teams:

- Improve campaign performance.
- Optimize marketing spending.
- Increase conversion rates.
- Monitor KPIs in real time.
- Make data-driven decisions.

---

## 📁 Repository Structure

```
marketing-funnel-powerbi-dashboard/
│
├── Marketing_Funnel_Dashboard.pbix
├── README.md
├── data/
│   └── funnel_cleaned.csv
├── images/
│   └── dashboard-overview.png
└── docs/
    └── project-summary.pdf
```

---

## 🚀 Skills Demonstrated

- Data Cleaning
- Data Transformation
- Power Query
- DAX
- Data Modeling
- Interactive Dashboard Design
- KPI Development
- Marketing Analytics
- Business Intelligence
- Data Visualization
- Storytelling with Data

 Future Improvements

- Month-over-Month Lead Growth
- Quarter-over-Quarter Analysis
- Dynamic KPI Indicators
- Drill-through Pages
- Custom Tooltips
- Forecasting
- Marketing ROI Analysis
- Email: owinocollain@gmail.com

## ⭐ If you found this project useful

Please consider giving the repository a ⭐ to support my work.


# FUTURE_DS_03
