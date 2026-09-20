# Customer Shopping Behavior Analysis

**An end-to-end data analytics project: Python → MySQL → Power BI → Business Report**

---

## Table of Contents

- [Project Overview](#project-overview)
- [Business Objectives](#business-objectives)
- [Dataset](#dataset)
- [Tools and Technologies](#tools-and-technologies)
- [Methodology](#methodology)
- [Key Findings](#key-findings)
- [Business Recommendations](#business-recommendations)
- [Power BI Dashboard](#power-bi-dashboard)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Skills Demonstrated](#skills-demonstrated)
- [Author](#author)

---

## Project Overview

This project analyzes **3,900 customer purchase records** to uncover patterns in spending, product preferences, subscription behavior, and purchasing trends. The goal is to turn raw transaction data into clear, actionable business insights that support data-driven decision-making.

The workflow spans the full analytics lifecycle: data is cleaned and explored in Python, stored and queried in MySQL, visualized in an interactive Power BI dashboard, and summarized in a business report with recommendations.

**Raw Dataset → Python (EDA and Cleaning) → MySQL → SQL Analysis → Power BI Dashboard → Business Report (PDF)**

---

## Business Objectives

The analysis was designed to answer questions such as:

- Which product categories and individual products drive the most revenue?
- How do subscribers differ from non-subscribers in spending behavior?
- How does purchasing behavior vary across age groups?
- Which products depend most on discounts?
- Which payment methods and shipping types do customers prefer?
- Which customer segments are the most valuable?

---

## Dataset

| Attribute | Detail |
|---|---|
| File | `data/customer_shopping_Behaviour.csv` |
| Records | 3,900 |
| Columns | 18 |
| Missing values | 37 (all in `Review Rating`) |

The dataset captures the following information:

| Feature Group | Description |
|---|---|
| Customer demographics | Age and gender, used for segmentation and age-group analysis |
| Product details | Product, category, size, color, and season |
| Transaction details | Purchase amount, payment method, and shipping type |
| Customer behavior | Subscription status, previous purchases, and purchase frequency |
| Promotions | Discount usage |
| Feedback | Review ratings |

---

## Tools and Technologies

| Tool | Purpose |
|---|---|
| **Python** | Data loading, cleaning, feature engineering, and exploratory analysis |
| **Pandas** | Data manipulation and analysis |
| **MySQL** | Data storage and querying |
| **SQL** | Business analysis and insight generation |
| **Power BI** | Interactive dashboard and data visualization |
| **Microsoft Word / PDF** | Business report preparation and final documentation |

---

## Methodology

### 1. Data Loading and Inspection

The dataset was loaded into Python with Pandas and inspected for structure, data types, statistical summaries, missing values, and overall consistency.

### 2. Exploratory Data Analysis

EDA was used to understand customer demographics, purchase patterns, product categories, subscription behavior, payment preferences, review ratings, and discount usage.

### 3. Data Cleaning and Feature Engineering

- Imputed missing review ratings using the **median rating of each product category**
- Standardized column names
- Verified data consistency
- Created **customer age groups**
- Created **purchase-frequency features**
- Removed redundant columns

### 4. MySQL Integration and SQL Analysis

The cleaned DataFrame was loaded into MySQL, where SQL queries were used to answer targeted business questions:

| Analysis | Focus |
|---|---|
| Revenue by gender | Compares total revenue across gender groups |
| High-spending discount users | Identifies customers who use discounts yet still spend heavily |
| Top-rated products | Highlights products with the strongest review ratings |
| Shipping-type comparison | Compares purchasing behavior across shipping options |
| Subscribers vs. non-subscribers | Contrasts spending between the two groups |
| Discount-dependent products | Finds products that rely most on discounts |
| Customer segmentation | Groups customers by purchase behavior |
| Top products by category | Ranks leading products within each category |
| Repeat buyers and subscriptions | Explores the link between repeat purchasing and subscribing |
| Revenue by age group | Shows which age groups contribute the most revenue |

### 5. Power BI Dashboard

An interactive dashboard was built on top of the MySQL data to visualize the results. See [Power BI Dashboard](#power-bi-dashboard).

### 6. Business Report

Findings were documented in a structured report covering the project overview, dataset, data preparation, Python EDA, SQL analysis, dashboard, business insights, and recommendations. The report is exported as a PDF for documentation and portfolio use.

---

## Key Findings

- **Clothing** is the leading product category by total purchase amount.
- **Subscription adoption is low:** roughly **27%** of customers are subscribers, while about **73%** are non-subscribers.
- **Spending varies across age groups**, indicating that some segments are more valuable than others.
- **Revenue is concentrated:** a relatively small group of products accounts for a significant share of total purchase value.
- **Credit Card** is the leading payment method.

---

## Business Recommendations

| Recommendation | Rationale |
|---|---|
| **Increase subscription adoption** | With only about 27% of customers subscribed, converting existing customers is a clear growth opportunity. |
| **Develop customer loyalty programs** | Rewarding repeat buyers can strengthen retention and customer lifetime value. |
| **Review discount strategy** | Evaluate discount-dependent products to ensure promotions support, rather than erode, profitability. |
| **Promote top-rated and best-selling products** | Feature proven performers in campaigns and merchandising. |
| **Target high-revenue customer segments** | Focus marketing effort on the age groups and segments that contribute the most value. |

---

## Power BI Dashboard

The interactive dashboard provides a consolidated view of customer purchasing behavior. Users can apply filters to explore:

- Customer and purchase KPIs
- Purchase amount analysis
- Category performance
- Top 10 products
- Subscription status analysis
- Payment method analysis
- Age-group purchasing behavior

---

## Project Structure

```text
Customer_Behavior_Analysis/
│
├── data/
│   └── customer_shopping_Behaviour.csv
│
├── python/
│   └── Cleaning_And_EDA.ipynb
│
├── sql/
│   └── Customer_Behaviour_Analysis_Queries.sql
│
├── powerbi/
│   └── Customer_Behaviour_Analysis.pbix
│
├── report/
│   └── Customer Shopping Behaviour Analysis Final Report.pdf
│
└── README.md
```

---

## Getting Started

### Prerequisites

- Python 3.9 or higher
- Jupyter Notebook or JupyterLab
- MySQL Server (8.0 or higher recommended)
- Power BI Desktop (Windows), with [MySQL Connector/NET](https://dev.mysql.com/downloads/connector/net/) installed to connect to MySQL

### 1. Clone the Repository

```bash
git clone https://github.com/kabilan-analytics/Customer_Behavior_Analysis.git
cd Customer_Behavior_Analysis
```

### 2. Set Up the Python Environment

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
pip install pandas numpy matplotlib seaborn sqlalchemy pymysql jupyter
```

### 3. Run the Python Notebook

Open `python/Cleaning_And_EDA.ipynb` and run all cells to:

- Load the dataset
- Perform exploratory data analysis
- Clean the data and engineer features
- Load the cleaned data into MySQL

> **Note:** Before running the database step, update the MySQL connection details (host, user, password, and database name) in the notebook. Avoid committing credentials to version control.

### 4. Run the SQL Analysis

Open `sql/Customer_Behaviour_Analysis_Queries.sql` in your preferred MySQL client (for example, MySQL Workbench), connect to your database, and execute the queries.

### 5. Open the Power BI Dashboard

Open `powerbi/Customer_Behaviour_Analysis.pbix`. If needed, update the data source under **Home → Transform data → Data source settings**, then select **Refresh**.

### 6. View the Final Report

The complete project documentation is available at [`report/Customer Shopping Behaviour Analysis Final Report.pdf`](report/Customer%20Shopping%20Behaviour%20Analysis%20Final%20Report.pdf).

---

## Skills Demonstrated

| Area | Skills |
|---|---|
| Data analysis | Python, Pandas, Exploratory Data Analysis, Data Cleaning, Feature Engineering |
| Databases | MySQL, SQL Business Analysis |
| BI and visualization | Power BI, Data Visualization |
| Communication | Business Insights, Business Reporting, Documentation |

---

## Author

**KABILAN S**

- LinkedIn: linkedin.com/in/kabilan-s-754758260
- GitHub: https://github.com/kabilan-analytics
- Email: kabik9003@gmail.com
