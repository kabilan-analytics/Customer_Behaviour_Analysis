````markdown
# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior using 3,900 purchase records to identify patterns in customer spending, product preferences, subscription behavior, and purchasing trends.

The project follows an end-to-end data analytics workflow:

**Python → Data Cleaning & EDA → MySQL → SQL Analysis → Power BI Dashboard → Business Report → PDF**

The objective is to transform raw customer transaction data into meaningful business insights that can support data-driven decision-making.

---

## Dataset

The dataset contains **3,900 rows and 18 columns**.

Key information includes:

- Customer demographics
- Product and category details
- Purchase amount
- Subscription status
- Payment method
- Shipping type
- Review ratings
- Discount usage
- Previous purchases
- Purchase frequency
- Season, size, and color

The dataset initially contained 37 missing values in the `Review Rating` column.

---

## Tools & Technologies

- **Python** – Data loading, cleaning, feature engineering, and EDA
- **Pandas** – Data manipulation and analysis
- **MySQL** – Data storage and SQL analysis
- **SQL** – Business analysis and insight generation
- **Power BI** – Interactive dashboard and data visualization
- **Microsoft Word** – Business report preparation
- **PDF** – Final project documentation

---

## Project Workflow

### 1. Data Loading

The dataset was loaded into Python using Pandas.

Initial exploration was performed to understand:

- Dataset structure
- Data types
- Statistical summaries
- Missing values
- Data consistency

### 2. Exploratory Data Analysis

EDA was performed to understand:

- Customer demographics
- Purchase patterns
- Product categories
- Subscription behavior
- Payment preferences
- Review ratings
- Discount usage

### 3. Data Cleaning

The dataset was cleaned and prepared for analysis.

Key steps included:

- Handling missing review ratings
- Standardizing column names
- Checking data consistency
- Creating customer age groups
- Creating purchase-frequency features
- Removing redundant columns

Missing review ratings were imputed using the median rating of the respective product category.

### 4. MySQL Integration

The cleaned Pandas DataFrame was loaded into MySQL for structured SQL analysis.

SQL analysis included:

- Revenue by gender
- High-spending discount users
- Top-rated products
- Shipping-type comparison
- Subscribers vs. non-subscribers
- Discount-dependent products
- Customer segmentation
- Top products by category
- Repeat buyers and subscriptions
- Revenue by age group

### 5. Power BI Dashboard

An interactive Power BI dashboard was created to visualize the results of the analysis.

The dashboard includes:

- Customer KPIs
- Purchase amount analysis
- Category performance
- Subscription analysis
- Payment method analysis
- Top 10 products
- Age-group purchasing behavior
- Interactive filters

### 6. Business Report

The analysis was documented in a structured business report covering:

- Project overview
- Dataset description
- Data preparation
- Python EDA
- SQL analysis
- Power BI dashboard
- Business insights
- Business recommendations

The final report was exported as a PDF for project documentation and portfolio presentation.

---

## Key Results

The analysis generated several business insights:

- **Clothing** is the leading product category by purchase amount.
- Approximately **27% of customers are subscribers**, while around 73% are non-subscribers.
- Customer spending varies across different age groups.
- A relatively small group of products contributes significantly to total purchase value.
- **Credit Card** is the leading payment method in the dataset.

---

## Business Recommendations

Based on the analysis, the project provides recommendations around:

- Increasing subscription adoption
- Developing customer loyalty programs
- Reviewing discount strategies
- Promoting top-rated and best-selling products
- Targeting high-revenue customer segments

---

## Dashboard

The Power BI dashboard provides an interactive view of customer purchasing behavior.

Users can explore the data using filters and analyze:

- Customer and purchase KPIs
- Category performance
- Top 10 products
- Subscription status
- Payment methods
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
````

---

## How to Run

### 1. Clone the Repository

```bash
git clone <https://github.com/kabilan-analytics/Customer_Behaviour_Analysis>
cd Customer_Behaviour_Analysis
```

### 2. Install Python Libraries

```bash
pip install pandas numpy matplotlib seaborn sqlalchemy pymysql jupyter
```

### 3. Run the Python Notebook

Open:

```text
Cleaning_And_EDA.ipynb
```

Run the notebook to:

* Load the dataset
* Perform EDA
* Clean the data
* Create required features
* Load the cleaned data into MySQL

### 4. Run SQL Analysis

Open:

```text
sql/Customer_Behaviour_Analysis_Queries.sql
```

Connect to your MySQL database and execute the queries.

### 5. Open the Power BI Dashboard

Open:

```text
powerbi/Customer_Behaviour_Analysis.pbix
```

Update the MySQL connection if required and refresh the dataset.

### 6. View the Final Report

The completed project documentation is available at:

```text
report/Customer Shopping Behaviour Analysis Final Report.pdf
```

---

## Skills Demonstrated

* Python for Data Analysis
* Pandas
* Exploratory Data Analysis
* Data Cleaning
* Feature Engineering
* MySQL
* SQL Business Analysis
* Power BI
* Data Visualization
* Business Insights
* Business Reporting
* End-to-End Data Analytics

---

## Project Outcome

This project demonstrates how raw customer transaction data can be transformed into a structured analytical solution using Python, SQL, and Power BI, followed by business-focused reporting and documentation.

### End-to-End Workflow

**Raw Dataset → Python EDA → Data Cleaning → MySQL → SQL Analysis → Power BI Dashboard → Business Insights → PDF Report**

```
```
