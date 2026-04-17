## Customer Shopping Behavior Analysis

## Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases to guide strategic business decisions. The goal is to leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies. The analysis follows a comprehensive data pipeline: preparing and cleaning data in **Python**, performing structured analysis in **PostgreSQL**, and building an interactive dashboard in **Power BI**.

-----

## Problem

A leading retail company needs to better understand its customers' shopping behavior to improve sales and long-term loyalty. Management has identified a critical challenge:

  * Noticing changes in purchasing patterns across demographics, product categories, and sales channels.
  * Identifying which specific factors, such as discounts, reviews, seasons, or payment preferences, drive consumer decisions and repeat purchases.

Failure to leverage this data effectively puts the organization at risk of:

  * Missing key trends in customer engagement.
  * Lacking data-driven insights for product and marketing optimization.
  * Inefficient strategy development for customer retention.

-----

## Methodology

### 1\. Data Preparation & Exploratory Analysis (Python)

Developed a data cleaning and transformation pipeline using **pandas** to ensure data quality.

  * **Initial Exploration**: Used `df.info` and `describe()` to check structure and summary statistics.
  * **Cleaning**: Imputed missing values in the Review Rating column using category medians and renamed columns to snake\_case for readability.
  * **Feature Engineering**: Created an `age_group` column by binning ages and established a `purchase_frequency_days` feature.

### 2\. Database Integration & SQL Analysis

  * **Integration**: Connected the Python script to **PostgreSQL** to load the cleaned DataFrame into a structured format for analysis.
  * **Business Transactions**: Performed structured analysis to answer key business questions, including revenue by gender, top products by rating, and customer segmentation.

-----

### Dashboard Visualization

The analysis was finalized into an interactive Power BI dashboard to present insights visually for stakeholders.

[**View Live Power BI Dashboard**](https://app.powerbi.com/view?r=eyJrIjoiOTI3MTNlYjQtZGI2My00OGU4LTllNTktOTM4MTkzZjEzNjhhIiwidCI6Ijg4ZDQ0NWU1LWU5YjAtNGNkMy04MTVmLTQwZjhhMzAwOWI0MiIsImMiOjEwfQ%3D%3D)
-----

### 3\. Key SQL Business Queries & Results

  * **Revenue by Gender**: Identified that Male customers generated $157,890 while Female customers generated $75,191.
  * **Customer Segmentation**: Classified the database into **Loyal (3,116)**, **Returning (701)**, and **New (83)** segments.
  * **Subscribers vs. Non-Subscribers**: Found that while non-subscribers are the majority (2,847), subscribers have a comparable average spend of $59.49.

-----

## Results

### Performance Benchmarks (EDA Summary)

| Metric | Value |
| :--- | :--- |
| Total Purchases | 3,900 |
| Average Purchase | $59.76 |
| Average Review Rating | 3.75 |
| Top Category | Clothing |

-----

## Strategic Business Insights

The analysis revealed critical areas for growth:

  * **Demographic Opportunities**: Young Adults represent the highest revenue contribution at $62,143.
  * **Subscription Drivers**: Checked whether customers with more than 5 previous purchases are more likely to subscribe to target for conversion.
  * **Product Strategy**: Highlighting top-rated items like Gloves and Sandals can drive engagement.

## Scalable Forecasting Framework

Delivered a modular project structure that can be updated with:

  * New transactional data via the Python ETL script.
  * Advanced SQL queries to track changing loyalty segments.
  * Real-time dashboard updates in Power BI to support stakeholder decision-making.

-----

## Tech Stack

| Category | Tools |
| :--- | :--- |
| **Data Processing** | Python (pandas, numpy) |
| **Database** | PostgreSQL |
| **Visualization** | Power BI |
| **Integration** | SQLAlchemy (Python-to-SQL connection) |

-----

## Key Skills Demonstrated

  * Data Preparation & ETL
  * SQL Business Logic & Querying
  * Customer Segmentation & Profiling
  * Interactive Dashboard Design
  * Business Data Storytelling
  * GitHub Repository Management
