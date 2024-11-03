# Organic-Grocery-Association-Rules
# Sales Analysis and Association Rule Mining

## Overview

This repository contains a Jupyter Notebook that performs sales data analysis and discovers association rules using the Apriori algorithm. The analysis is aimed at understanding customer purchasing behavior by identifying frequently bought products together.

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

##Key Features

*Data Cleaning: The notebook processes the sales data by removing unnecessary columns and checking for missing values.

*Product Encoding: Products are encoded to facilitate the application of the Apriori algorithm.

Frequent Itemset Mining: The Apriori algorithm is employed to identify frequently bought product combinations based on a defined minimum support threshold.

Association Rule Generation: Association rules are generated from the frequent itemsets, providing insights into product associations with a focus on confidence metrics.

Visualization: Histograms and other visualizations are included to present the distribution of order sizes and the results of the analysis.


The results, including frequent itemsets and association rules, will be saved as Excel files (frequent_itemsets (Organic).xlsx and association_rules (Organic).xlsx) in the directory.

Results
The notebook will output:

A histogram visualizing the distribution of product quantities per order.
A list of frequent itemsets with their support values.
Association rules including antecedents and consequents with confidence scores.
