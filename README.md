# 🏦 Bank Customer Segmentation & Risk Analytics | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![DAX](https://img.shields.io/badge/DAX-Measures-blue)
![Data Analytics](https://img.shields.io/badge/Data%20Analytics-Project-green)
![RFM Analysis](https://img.shields.io/badge/RFM-Customer%20Segmentation-purple)

## 📌 Project Overview

The **Bank Customer Segmentation & Risk Analytics** project is an end-to-end **Power BI data analytics project** designed to analyze customer demographics, transaction behavior, customer value, RFM-based segmentation, and risk indicators.

The project transforms customer and transaction-level banking data into an interactive Power BI dashboard that enables users to explore **customer profiles, transaction patterns, customer segments, revenue/value indicators, and risk distribution**.

The dashboard is designed from a business-analysis perspective to demonstrate how Power BI, data modeling, DAX, and customer segmentation techniques can be used to support data-driven decision-making.

---

# 🎯 Business Problem

Banks and financial institutions manage large volumes of customer and transaction data.

Without proper analysis, it can be difficult to answer questions such as:

* Who are the most valuable customers?
* Which customer segments are highly active?
* What are the transaction patterns across different customer groups?
* Which customers may require additional attention from a risk perspective?
* How does customer behavior vary by age, gender, location, and transaction activity?
* Which customer segments contribute the greatest monetary value?

This project addresses these questions through an interactive Power BI analytical solution.

---

# 🚀 Project Objectives

The primary objectives of this project are to:

* Analyze customer demographics and account characteristics.
* Understand transaction behavior and trends.
* Analyze transaction amount and account balance patterns.
* Segment customers using **RFM (Recency, Frequency, Monetary) analysis**.
* Identify high-value and potentially at-risk customer segments.
* Develop risk-related indicators for customer analysis.
* Create interactive Power BI dashboards with slicers and KPIs.
* Convert raw transactional data into meaningful business insights.
* Demonstrate practical Power BI, DAX, data modeling, and analytical skills.

---

# 📊 Dataset

The dataset contains customer and banking transaction information.

### Key fields include:

| Field                | Description                   |
| -------------------- | ----------------------------- |
| `TransactionID`      | Unique transaction identifier |
| `CustomerID`         | Unique customer identifier    |
| `CustomerDOB`        | Customer date of birth        |
| `CustGender`         | Customer gender               |
| `CustLocation`       | Customer location             |
| `CustAccountBalance` | Customer account balance      |
| `TransactionDate`    | Date of transaction           |
| `TransactionTime`    | Time of transaction           |
| `TransactionAmount`  | Transaction amount in INR     |

The dataset contains a large number of customer and transaction records and is used to perform customer-level and transaction-level analysis.

---

# 🏗️ Data Modeling

The project uses Power BI's data modeling capabilities to organize customer and transaction information.

The analytical model includes customer-level information, transaction information, customer summary information, and supporting date structures.

### Conceptual model

```text
                 ┌─────────────────────┐
                 │     Customers       │
                 │                     │
                 │ CustomerID          │
                 │ Gender              │
                 │ Location            │
                 │ Age                 │
                 │ Account Balance     │
                 └──────────┬──────────┘
                            │
                            │ CustomerID
                            │
                 ┌──────────▼──────────┐
                 │    Transactions     │
                 │                     │
                 │ TransactionID       │
                 │ CustomerID          │
                 │ TransactionDate     │
                 │ TransactionAmount   │
                 │ TransactionTime     │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Customer Analysis   │
                 │                     │
                 │ RFM Scores          │
                 │ Customer Segment     │
                 │ Revenue / Value     │
                 │ Risk Indicators     │
                 └─────────────────────┘
```

The final Power BI model is used to support customer demographics, transaction analysis, RFM segmentation, and risk analytics.

---

# 📈 Dashboard Structure

The Power BI report is organized into four major analytical areas.

## 1. 👥 Customer Demographics

This section provides an overview of the customer base.

### KPIs and analysis include:

* Total Customers
* Average Age
* Total Transactions
* Gender distribution
* Male customers
* Female customers
* Transgender customers
* Unknown/blank gender records
* Unique customer locations
* Customer age groups

### Business Questions

* How large is the customer base?
* What is the customer age distribution?
* What is the gender composition?
* How geographically diverse are customers?
* Which age groups represent the largest customer populations?

### Business Value

This analysis helps understand the overall customer profile and provides a foundation for customer segmentation and targeted business strategies.

---

# 💳 2. Transaction Behavior Analysis

The transaction analysis section focuses on customer transaction activity and monetary behavior.

### Key metrics include:

* Total Transactions
* Average Account Balance
* Transaction Volume
* Average Transaction Amount
* Transaction trends over time
* Transaction amount by age group
* Day-level transaction analysis
* Time-based transaction analysis

### Business Questions

* How frequently are customers transacting?
* What is the average transaction amount?
* How does transaction behavior vary by age group?
* How does transaction activity change over time?
* Which customer groups demonstrate higher transaction activity?

### Business Value

Transaction analysis helps identify behavioral patterns and supports understanding of customer engagement and transaction activity.

---

# 🎯 3. RFM Customer Segmentation

One of the core analytical components of this project is **RFM analysis**.

RFM stands for:

| Metric            | Meaning                                        |
| ----------------- | ---------------------------------------------- |
| **Recency (R)**   | How recently a customer made a transaction     |
| **Frequency (F)** | How frequently a customer transacts            |
| **Monetary (M)**  | How much monetary value the customer generates |

Customers are assigned scores based on these three dimensions.

### RFM Framework

```text
                 Customer Transactions
                         │
                         ▼
              ┌─────────────────────┐
              │    RFM Analysis     │
              └──────────┬──────────┘
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
      Recency        Frequency       Monetary
          │              │              │
          ▼              ▼              ▼
       R Score         F Score        M Score
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                Customer Segments
```

---

## 🧩 Customer Segments

The project categorizes customers using RFM scores.

### 🏆 Champions

Customers with:

* High Recency score
* High Frequency score

These represent highly active and valuable customers.

### 💙 Loyal Customers

Customers with:

* Strong Recency
* Strong Frequency

These customers demonstrate consistent engagement.

### ⚠️ At Risk

Customers with:

* Low Recency
* High Frequency

These customers were historically active but may require additional engagement.

### 🔴 Lost Customers

Customers with:

* Low Recency
* Low Frequency

These customers show lower recent activity and engagement.

### 💰 High Spenders

Customers with:

* High Monetary score

These customers contribute relatively high monetary value.

### 🔹 Others

Customers who do not fall into the primary segmentation categories.

---

# 💰 4. Profitability & Risk Analytics

The final analytical area combines customer value indicators with risk-oriented analysis.

### Key analysis includes:

* Total Customer Revenue
* Average Credit Score
* High-Risk Customer Count
* Total Monetary Value
* Risk distribution
* Customer segment vs risk
* Account balance vs risk
* Value Score
* High-revenue / high-risk customer analysis

### Risk Analysis Framework

```text
Customer Data
      │
      ├── Account Balance
      ├── Transaction Activity
      ├── RFM Scores
      └── Credit Score
             │
             ▼
       Risk Indicators
             │
             ▼
       Risk Distribution
             │
             ▼
   Customer-Level Analysis
```

> **Note:** The credit score used in this project is a simulated analytical field created for dashboard/risk-analysis purposes. It should not be interpreted as an actual bank-issued credit score.

---

# 🧮 DAX & Analytical Measures

DAX was used to create analytical measures and customer-level calculations required for the dashboard.

Examples of analytical metrics include:

```text
Total Customers
Total Transactions
Average Age
Average Account Balance
Average Transaction Amount
Total Revenue
RFM Scores
Customer Segment
Average Credit Score
High Risk Customers
Total Monetary Value
Value Score
```

### Example RFM segmentation logic

The customer segmentation follows business rules based on RFM scores:

```text
Champions
→ R_Score = 5 AND F_Score >= 4

Loyal
→ R_Score >= 4 AND F_Score >= 3

At Risk
→ R_Score <= 2 AND F_Score >= 3

Lost
→ R_Score <= 2 AND F_Score <= 2

High Spenders
→ M_Score >= 4

Others
→ Remaining customers
```

This approach converts numerical RFM scores into business-friendly customer segments.

---

# 🎛️ Interactive Dashboard Features

The dashboard supports interactive exploration using filters and slicers.

### Available analytical filters include:

* Customer Segment
* Gender
* Age Group
* Location

Users can combine filters to analyze specific customer groups and compare customer behavior across different dimensions.

---

# 📸 Dashboard Preview

## Customer Demographics

![Customer Demographics](screenshots/01_customer_demographics.png)

---

## Transaction Behavior

![Transaction Behavior](screenshots/02_transaction_analysis.png)

---

## RFM Customer Segmentation

![RFM Segmentation](screenshots/03_rfm_segmentation.png)

---

## Profitability & Risk Analysis

![Risk Analysis](screenshots/04_risk_analysis.png)

> **Note:** Replace the image paths above with the actual screenshots uploaded to the `screenshots` folder.

---

# 🔍 Key Business Questions

This dashboard is designed to answer questions such as:

### Customer Analysis

* How many customers are in the database?
* What is the average customer age?
* What is the gender distribution?
* Which locations have the highest customer concentration?

### Transaction Analysis

* How many transactions have occurred?
* What is the average transaction amount?
* How does transaction activity change over time?
* Which age groups have higher transaction values?

### Customer Segmentation

* Who are the most active customers?
* Which customers are loyal?
* Which customers are at risk?
* Which customers have been lost?
* Who are the high spenders?

### Risk Analysis

* What is the average credit score?
* How many customers are classified as high risk?
* How does risk vary by customer segment?
* What is the relationship between account balance and risk?
* Which high-value customers also show high-risk indicators?

---

# 💡 Business Insights

The project enables organizations to move from raw transaction data to actionable customer intelligence.

Potential business applications include:

### Customer Retention

Identify **At Risk** and **Lost** customers for targeted retention campaigns.

### Customer Loyalty

Identify **Champions** and **Loyal Customers** and develop personalized engagement strategies.

### Revenue Optimization

Identify **High Spenders** and high-monetary-value customers.

### Risk Monitoring

Analyze customer segments alongside risk indicators to identify customers requiring additional attention.

### Customer Strategy

Use demographic and transaction patterns to support targeted products, services, and campaigns.

---

# 🛠️ Tools & Technologies

| Technology        | Purpose                                          |
| ----------------- | ------------------------------------------------ |
| **Power BI**      | Dashboard development and visualization          |
| **Power Query**   | Data transformation and preparation              |
| **DAX**           | Measures, calculations, scoring and segmentation |
| **Excel/CSV**     | Source data                                      |
| **Data Modeling** | Relationships and analytical model               |
| **RFM Analysis**  | Customer segmentation                            |

---

# 📁 Repository Structure

```text
Bank-Customer-Segmentation-PowerBI/
│
├── README.md
│
├── screenshots/
│   ├── 01_customer_demographics.png
│   ├── 02_transaction_analysis.png
│   ├── 03_rfm_segmentation.png
│   └── 04_risk_analysis.png
│
├── documentation/
│   └── Bank_Customer_Segmentation_Project.pdf
│
├── data/
│   └── sample_bank_customer_data.csv
│
└── dax/
    └── DAX_Measures.md
```

---

# 📂 Power BI File

The complete `.pbix` file is maintained separately because the Power BI project file exceeds GitHub's standard browser upload limit.

The GitHub repository therefore contains:

* Dashboard screenshots
* Project documentation
* Sample dataset
* Key DAX measures
* Project methodology
* Business insights

### Power BI File

🔗 **[Download / View the Power BI `.pbix` file](YOUR_PBIX_LINK_HERE)**

> Replace `YOUR_PBIX_LINK_HERE` with your actual external file-sharing link.

---

# 📄 Documentation

Detailed project documentation covers:

* Business problem
* Dataset description
* Data preparation
* Data modeling
* DAX calculations
* RFM methodology
* Customer segmentation
* Risk analysis
* Dashboard design
* Business insights

Documentation:

**`documentation/Bank_Customer_Segmentation_Project.pdf`**

---

# 📊 Analytical Workflow

The overall project workflow can be summarized as:

```text
Raw Banking Data
       │
       ▼
Data Preparation
       │
       ▼
Data Cleaning & Transformation
       │
       ▼
Data Modeling
       │
       ▼
DAX Measures
       │
       ▼
Customer & Transaction Analysis
       │
       ▼
RFM Analysis
       │
       ▼
Customer Segmentation
       │
       ▼
Risk & Value Analysis
       │
       ▼
Interactive Power BI Dashboard
       │
       ▼
Business Insights
```

---

# 📌 Project Highlights

* Built an interactive **Power BI banking analytics dashboard**.
* Analyzed customer demographics and transaction behavior.
* Implemented **RFM-based customer segmentation**.
* Created customer segments including Champions, Loyal, At Risk, Lost, and High Spenders.
* Developed DAX-based KPIs and analytical measures.
* Created risk and value indicators.
* Analyzed customer behavior across age, gender, location, and transaction dimensions.
* Designed an interactive dashboard using Power BI slicers and visualizations.
* Converted large-scale customer transaction data into business-oriented insights.

---

# 🎓 Skills Demonstrated

This project demonstrates practical experience in:

### Data Analytics

* Exploratory Data Analysis
* Customer Analytics
* Transaction Analysis
* Revenue Analysis
* Risk Analytics

### Power BI

* Data Modeling
* Power Query
* DAX
* KPI Development
* Interactive Visualizations
* Slicers and Filters
* Dashboard Design

### Business Analytics

* Customer Segmentation
* RFM Analysis
* Customer Retention
* Customer Value Analysis
* Risk Identification
* Business Decision Support

---

# 🚀 Future Enhancements

Potential improvements to the project include:

* Connect Power BI directly to a SQL database.
* Implement automated data refresh.
* Add advanced customer lifetime value analysis.
* Add cohort analysis.
* Add customer churn prediction using Machine Learning.
* Develop predictive risk modeling.
* Add geographic customer analysis.
* Add time-series forecasting.
* Improve the risk scoring framework using real financial risk variables.
* Implement row-level security for role-based dashboard access.

---

# 👨‍💻 Author

## Madhu Kurakula

**Associate Data Analyst | SQL | Python | Power BI | Data Analytics**

This project is part of my data analytics portfolio and demonstrates practical skills in **Power BI, DAX, data modeling, customer segmentation, transaction analytics, and business intelligence**.

---

## ⭐ If you found this project useful

If you found this project useful or interesting, consider giving the repository a ⭐.

Feel free to explore the dashboard screenshots, DAX calculations, documentation, and analytical methodology.
