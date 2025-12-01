# Olist E-Commerce Sales & Logistics Dashboard

## Project Overview

This Power BI dashboard provides a comprehensive analysis of the Olist E-commerce marketplace, a Brazilian platform connecting small businesses to customers. The project analyzes a dataset of 100,000+ orders placed between 2016 and 2018.

The dashboard is designed to help stakeholders monitor sales performance, optimize logistics, and understand customer behavior. It highlights key performance indicators (KPIs), seasonal trends, payment preferences, and delivery efficiency.

The project demonstrates skills in:
- Data Modeling (Star Schema design)
- Power Query (ETL & Data Cleaning)
- DAX (Complex measures & calculated columns)
- Data Visualization (Interactive charts & maps)
- Storytelling (Actionable insights)

## Dashboard Preview

![Dashboard Screenshot](https://github.com/user-attachments/assets/your-image-link-here)

## Features

### 1. Key KPIs
- Total Revenue: Global sales volume over the selected period.
- Total Orders: Count of unique orders placed.
- Average Order Value (AOV): Revenue per transaction.
- Average Delivery Days: Time taken from order approval to customer delivery.
- Freight Ratio: Percentage of total cost attributed to shipping.

### 2. Visual Insights
- Sales Trends: Monthly and yearly revenue tracking (identifying Seasonality/Black Friday).
- Geographic Distribution: Heatmap of sales by State and City (using Geolocation data).
- Category Performance: Top 10 product categories by revenue and volume.
- Payment Analysis: Breakdown of payment methods (Credit Card, Boleto, Voucher).
- Logistics Performance: Comparison of Estimated vs. Actual Delivery dates.

### 3. Interactive Filters
- Date Slicer: Filter by Year, Quarter, and Month.
- Region Filter: Drill down by State (UF) or City.
- Product Category: Filter specific market segments (e.g., Health & Beauty, Tech).

## Tools Used

- Microsoft Power BI Desktop: Dashboarding and visualization.
- Power Query: Merging 9 distinct datasets and handling null values.
- DAX (Data Analysis Expressions): Creating measures for time-intelligence and ratios.
- Excel/CSV: Source data format.

## Dataset Description

The dataset consists of 9 relational CSV files provided by Olist. It covers the entire order journey: from purchase to payment, shipping, and customer review.

Below is the data dictionary explaining the source files used in the Data Model.

## Data Dictionary

| Table Name | Description |
|:---|:---|
| olist_orders_dataset | Core table containing Order ID, status, timestamps (purchase, approval, delivery). |
| olist_order_items_dataset | Details of items within an order (Product ID, Price, Freight Value, Seller ID). |
| olist_products_dataset | Product metadata including category name, weight, and dimensions. |
| olist_customers_dataset | Customer demographic info (City, State, Zip Code). |
| olist_order_payments_dataset | Payment details (Method: Credit Card/Voucher, Installments, Transaction Value). |
| olist_order_reviews_dataset | Customer satisfaction data (Review Score 1-5, Comments). |
| olist_sellers_dataset | Seller location and ID information. |
| olist_geolocation_dataset | Latitude and Longitude coordinates for mapping customers and sellers. |
| product_category_translation | Translations of category names from Portuguese to English. |

## Key Insights

### 1. Geographic Concentration
The Southeast region (especially Sao Paulo) accounts for the vast majority of orders and revenue, indicating a need for logistics optimization in other regions.

### 2. Seasonality & Peaks
There is a significant spike in sales during Black Friday (November), requiring scaled-up inventory and server capacity during Q4.

### 3. Delivery Efficiency
While most orders arrive on time, there is a visible gap between Estimated Delivery Date and Actual Delivery Date in northern states, often leading to lower review scores.

### 4. Payment Preferences
Credit Cards are the dominant payment method, with a high usage of installments (Parcelado), suggesting customers prefer spreading costs for higher-value items.

### 5. Product Category Leaders
Categories like "Bed, Bath & Table" and "Health & Beauty" consistently lead in volume, while "Tech/Electronics" have higher average ticket sizes.

### 6. Freight Impact
High freight costs relative to product price (especially for cheaper items) negatively correlate with conversion rates and customer satisfaction.

## Recommendations

### 1. Logistics Optimization
Establish warehousing partnerships in the North/Northeast regions to reduce delivery times and freight costs, thereby improving customer satisfaction outside of Sao Paulo.

### 2. Inventory Planning
Sellers should use the seasonality data to stock up heavily on "Bed & Bath" and "Decor" items specifically for the Q4 Black Friday rush.

### 3. Payment Incentives
Since Credit Card installments are popular, offer interest-free installment promotions to increase the Average Order Value (AOV).

### 4. Seller Quality Control
Identify sellers with consistently late shipping or poor reviews and provide training or penalties to maintain platform reputation.

### 5. Marketing Focus
Target marketing campaigns in under-penetrated states (like Rio de Janeiro or Minas Gerais) where logistics are stable but order volume is below potential.

