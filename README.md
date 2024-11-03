# Organic-Grocery-Association-Rules
# Sales Analysis and Association Rule Mining

## Overview

This repository contains a Colab Notebook that performs sales data analysis and discovers association rules using the Apriori algorithm. The analysis is aimed at understanding customer purchasing behavior by identifying frequently bought products together.

## Requirements

Make sure to have the following Python packages installed:

- pandas
- numpy
- matplotlib
- seaborn
- mlxtend
- scikit-learn
- scipy

The main data source is a CSV file named sales.csv, which should be placed in the same directory as the notebook. The data includes information on product sales, which is utilized for the analysis.

## Key Features

**Data Cleaning** : The notebook processes the sales data by removing unnecessary columns and checking for missing values.

**Product Encoding**: Products are encoded to facilitate the application of the Apriori algorithm.

**Frequent Itemset Mining**: The Apriori algorithm is employed to identify frequently bought product combinations based on a defined minimum support threshold.

**Association Rule Generation**: Association rules are generated from the frequent itemsets, providing insights into product associations with a focus on confidence metrics.

**Visualization**: Histograms and other visualizations are included to present the distribution of order sizes and the results of the analysis.


The results, including frequent itemsets and association rules, will be saved as Excel files (frequent_itemsets (Organic).xlsx and association_rules (Organic).xlsx) in the directory.

## Results
The notebook will output:

- A histogram visualizing the distribution of product quantities per order.
- A list of frequent itemsets with their support values.
- Association rules including antecedents and consequents with confidence scores.
![Order Size Dis](https://github.com/user-attachments/assets/d5367bdb-d987-4364-aa53-c26a25871e0e)



# Sales Forecasting Analysis

## Overview

This project involves analyzing and forecasting sales data using Python libraries such as Pandas, NumPy, Plotly, and Prophet. The goal is to visualize sales trends, understand seasonal patterns, and predict future sales quantities and revenues.

## Installation

To run this project, you need to have the following Python libraries installed:

- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- prophet
- plotly

Load your sales data from a CSV file. Ensure that the CSV file contains the required columns: order_id, quantity, order_total_products_price, order_delivery_cost, order_total_price, order_customer_type, and order_date.

Run the code to preprocess the data, visualize sales trends, and generate forecasts.

The visualizations will display daily and monthly sales trends, moving averages, and time series decompositions.

- **Data Preprocessing**
The data is first read from a CSV file and grouped by order_id, summing the quantity.
The order_date is converted to a datetime format for easier analysis.

- Specific **dates & orders** had to be filtered out to refine the dataset.

- **Sales Visualization**
Daily and monthly sales trends are visualized using line plots.
Rolling averages (7-day and 3-month) are calculated to smooth the sales data for better insight.

- **Time series decomposition** is performed to extract trend, seasonal, and residual components from the sales data.
Forecasting

- **The Prophet** library is utilized to forecast future sales based on historical data.

- Historical data is prepared, and the model is fit to make predictions for the next 90 days.

- Confidence intervals for the forecast are also displayed in the visualizations.

## Conclusion
This project provides a comprehensive analysis of sales data, allowing for insightful visualizations and robust forecasting. You can modify the code to suit different datasets or forecasting needs.

Some Results:
![newplot (1)](https://github.com/user-attachments/assets/a0675992-a205-438d-b291-244212106e50)

![No  of order per day  plt](https://github.com/user-attachments/assets/de27ed62-1721-4212-90d9-b92cbb4fd295)

![Sales Forcast Plt](https://github.com/user-attachments/assets/4e329257-af0c-4af4-9bd6-ea687581e393)


