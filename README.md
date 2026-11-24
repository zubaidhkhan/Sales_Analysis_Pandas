A beginner-friendly exploratory data analysis (EDA) project that builds a sales dataset with pandas, performs data quality checks, derives revenue metrics, summarizes performance by product and category, and visualizes the results with Matplotlib.

Table of Contents
Project Overview
Key Insights
Dataset
Analysis Workflow
Visualizations
Tech Stack
Getting Started
Project Structure
Limitations and Future Work
Author
Project Overview

The goal of this project is to demonstrate core data analysis skills in Python:

Constructing and inspecting a tabular dataset with pandas.DataFrame
Checking data quality (missing values, duplicates, structure)
Engineering a derived metric (Revenue = Quantity × Price)
Aggregating data with groupby to answer business questions
Communicating findings with clear, labelled charts

The analysis is written as a Jupyter Notebook so each step is documented, reproducible, and easy to follow.
Analysis Performed
Built a DataFrame of 10 orders with 5 columns (Order_ID, Product, Category, Quantity, Price).
Checked data quality: no missing values, no duplicate rows.
Created a Revenue column (Quantity × Price).
Calculated totals: total revenue and total unit price.
Grouped by product to compare revenue.
Grouped by category to compare units sold.
Plotted two bar charts: revenue by product and quantity by category.
Key Results
Total revenue: ₹3,51,000 across 10 orders, averaging ₹35,100 per order.
Total units sold: 29.
Product	Units	Revenue	Share of Revenue
Laptop	6	₹3,00,000	85.5%
Monitor	3	₹36,000	10.3%
Keyboard	5	₹7,500	2.1%
Mouse	15	₹7,500	2.1%
Category	Units	Revenue	Share of Revenue
Electronics	9	₹3,36,000	95.7%
Accessories	20	₹15,000	4.3%
Insights
Laptops dominate revenue. Six laptop units bring in 85% of total revenue, because each one sells for ₹50,000.
Volume and revenue point in opposite directions. Mice have the most units sold (15) but tie with keyboards for the lowest revenue. Accessories sell the most units but earn only about 4% of revenue.
Price tiers drive results more than order count. Revenue depends mainly on unit price: laptops (₹50,000) and monitors (₹12,000) make up nearly all revenue, while mice (₹500) and keyboards (₹1,500) contribute very little.
The business depends on a few high-value sales. Losing one laptop order would cut revenue by roughly a third in this dataset.
Caveats
The dataset has only 10 synthetic records, so these patterns illustrate the method rather than reveal real business trends.
The "Total Price" figure (₹1,78,500) sums unit prices across orders, which isn't a meaningful business metric. I'd leave it out of any summary you show recruiters.
