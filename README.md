# Customer Segmentation

## Introduction
This project presents a comprehensive analysis of retail sales data using advanced clustering algorithms to segment customers based on their behavior. The goal is to develop personalized marketing strategies and enhance customer engagement. By leveraging RFM (Recency, Frequency, Monetary) analysis, K-means and DBSCAN clustering, and cohort analysis, we provide deep insights into customer segments and their lifetime value.

## Table of Contents
- [Introduction](#introduction)
- [Data Overview](#data-overview)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [RFM Analysis](#rfm-analysis)
- [Clustering Analysis](#clustering-analysis)
- [Cohort Analysis](#cohort-analysis)
- [Cluster Profiling](#cluster-profiling)
- [Top Customers Analysis](#top-customers-analysis)
- [Customer Lifetime Value (CLV) Analysis](#customer-lifetime-value-clv-analysis)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Data Overview
The project uses the "Online Retail" dataset, which contains transactional data from a UK-based online retail store. The dataset includes information such as invoice numbers, product details, quantities, prices, customer IDs, and transaction dates.

## Data Cleaning and Preprocessing
- Handling missing values in 'Description' and 'CustomerID' columns
- Removing duplicate entries
- Outlier detection and removal using the Interquartile Range (IQR) method
- Feature engineering: Creating 'TotalPrice' column
- Converting 'InvoiceDate' to datetime format

## Exploratory Data Analysis (EDA)
The EDA process involves analyzing the distribution of key variables such as purchase frequency, monetary value, and recency. Visualizations are created to understand patterns and relationships in the data.

## RFM Analysis
RFM (Recency, Frequency, Monetary) analysis is performed to segment customers based on:
- Recency: Days since last purchase
- Frequency: Number of purchases
- Monetary: Total amount spent
The RFM values are log-transformed to handle skewness in the data.

## Clustering Analysis
Two clustering algorithms are employed:
1. K-means: Optimal number of clusters determined using silhouette score
2. DBSCAN: For handling non-spherical clusters and identifying outliers

Results are visualized using Principal Component Analysis (PCA) for dimensionality reduction.

## Cohort Analysis
Cohort analysis is performed to understand customer retention and behavior over time. A heatmap visualization shows the retention rates for different customer cohorts.

## Cluster Profiling
Detailed profiles of each cluster are generated, including:
- Summary statistics for Recency, Frequency, and Monetary values
- Top 5 customers in each segment

## Top Customers Analysis
The top 10 customers are identified based on their Customer Lifetime Value (CLV).

## Customer Lifetime Value (CLV) Analysis
CLV is calculated using a simple formula: (Frequency * Monetary) / Recency. This provides an additional metric for evaluating customer value beyond RFM.

## Installation
To run this project, you need to install the following Python libraries:
```
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
```

## Usage
1. Ensure you have the "Online Retail.xlsx" file in the specified directory.
2. Run the main script:
   ```
   python customer_segmentation_project.py
   ```
3. The script will generate visualizations and output analysis results to the console.

## Contributing
Contributions to this project are welcome. Please fork the repository and submit a pull request with your proposed changes.

## License
MIT License

Copyright (c) 2024 Tobi-M-Data

## Contact
tobimautin@gmail.com

## Full Project Documentation
For a detailed report on the project, including all analyses and findings, please refer to the Full Project Documentation.
