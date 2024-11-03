# Organic-Grocery-Association-Rules
# Project Title: Association Rule Mining and Sales Trend Prediction

## Overview
This project aims to extract association rules from transaction data and predict sales trends for the **Organic Online Grocery Store** using a dataset containing transactions from June 1, 2024, to September 15, 2024.

## Dataset
The dataset is provided in a CSV format and includes the following columns:
- **order_id**: Unique identifier for each order.
- **product_id**: Identifier for the products purchased.
- **quantity**: Number of items purchased for each product.
- **order_date**: Date when the order was placed.
- **order_total_products_price**: Total price for products in the order.

### Data Preparation
The raw data contained multiple rows for orders with more than one product. To prepare the dataset for analysis, the following steps were taken:
1. **Grouped the data by `order_id`** to consolidate multiple products under a single order.
2. **Summed the `quantity`** for products within the same order while retaining unique product identifiers.

## Analysis
### Association Rule Mining
Using the **Apriori algorithm**, frequent itemsets were generated to identify products that are often purchased together. Key parameters included:
- **Minimum support**: 0.01
- **Minimum confidence**: 0.2

### Sales Trend Prediction
Trends in sales over the provided date range were analyzed to identify patterns and potential areas for growth.
