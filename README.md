# Customer Shopping Behavior Analysis

## Project Overview
his project provides a comprehensive analysis of consumer shopping patterns for a leading retail company[cite: 1, 2]. By leveraging data across 3,900 purchases, the analysis uncovers critical insights into spending habits, customer segmentation, and purchase drivers to optimize marketing and product strategies.

The project follows a full data pipeline: **Python** for cleaning and ETL, **PostgreSQL** for deep-dive transactional analysis, and **Power BI** for interactive visualization.

## Dataset Summary
The dataset consists of **3,900 rows** and **18 columns**, featuring:
* **Demographics:** Age, Gender, Location, and Subscription Status.
* **Transaction Details:** Item Purchased, Category, Purchase Amount, and Season.
* **Behavioral Data:** Review Ratings, Shipping Type, Previous Purchases, and Discount Usage.

## Tools & Technologies
* **Python (Pandas):** Data cleaning, missing value imputation, and feature engineering.
* **PostgreSQL:** Relational database management and complex business logic queries.
* **Power BI:** Interactive dashboard development for stakeholder reporting.
* **SQLAlchemy:** Integration for automated data loading from Python to SQL.

## Project Steps

### 1. Data Preparation & Cleaning (Python)
* **Initial EDA:** Explored data structure using `df.info()` and summary statistics.
* **Data Quality:** Imputed missing values in the Review Rating column using category medians and standardized column naming to snake_case.
* **Feature Engineering:** Created new features such as `age_group` (binned ages) and `purchase_frequency_days`.
* **Database Integration:** Successfully loaded the processed dataset into a PostgreSQL server for structured analysis.

### 2. Business Analysis (SQL)
Conducted deep-dive queries to answer key business questions:
* **Revenue Analysis:** Found that Male customers generated significantly higher total revenue ($157,890) compared to Female customers ($75,191).
* **Segmentation:** Classified the user base into New, Returning, and Loyal segments, identifying over 3,000 "Loyal" customers.
* **Purchase Drivers:** Analyzed the impact of shipping types and discount rates on purchase volume.

### 3. Data Visualization (Power BI)
Developed an interactive dashboard focusing on:
* High-level KPIs: Total Customers (3.9K), Average Spend ($59.76), and Average Rating (3.75).
* Category performance (Revenue and Sales volume).
* Customer distribution by Age Group and Subscription Status.

## Key Results & Insights
* **Young Adults** represent the highest revenue-generating age segment.
* **Clothing** is the top-selling category by both volume and revenue.
* Customers with more than 5 previous purchases show a notable distribution between subscribers and non-subscribers, indicating a massive opportunity for loyalty conversion.

## Business Recommendations
* **Targeted Marketing:** Focus campaigns on high-revenue age groups (Young Adults) and users preferring express shipping.
* **Subscription Growth:** Promote exclusive benefits to the 73% of customers who are currently non-subscribers.
* **Loyalty Retention:** Implement rewards programs specifically for the "Loyal" segment to maintain long-term engagement.

## Interactive Dashboard
[**View Live Power BI Dashboard**](https://app.powerbi.com/view?r=eyJrIjoiOTI3MTNlYjQtZGI2My00OGU4LTllNTktOTM4MTkzZjEzNjhhIiwidCI6Ijg4ZDQ0NWU1LWU5YjAtNGNkMy04MTVmLTQwZjhhMzAwOWI0MiIsImMiOjEwfQ%3D%3D)

## How to Run
1.  **Python:** Run the `cleaning_script.py` to process the raw CSV and load it into your local PostgreSQL instance.
2.  **SQL:** Execute the scripts in `analysis_queries.sql` to generate business insights.
3.  **Power BI:** Open the `.pbix` file to explore the interactive visualizations locally.
