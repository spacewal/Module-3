# Customer Lifetime Value Analysis README

## Overview
This Python script utilizes the Customer Lifetime Value (CLV) model to analyze customer purchase behavior and predict future spending. It segments customers into categories based on their transaction history to help businesses tailor their marketing strategies.

## Features
- **Data Preprocessing**: Converts 'Transaction Date' from object to datetime for accurate analysis and caps outliers in 'Total Price' to avoid data skew.
- **RFM Analysis**: Examines customer transaction data to establish the observation period for the CLV calculation.
- **CLV Calculation**: Determines the initial CLV without refining, and then refines the data for customers with more than one purchase.
- **Prediction Models**: Uses the BetaGeoFitter and GammaGammaFitter models to predict future purchases and calculate a six-month CLV.
- **Customer Segmentation**: Segments customers into 'Hibernating', 'Need Attention', 'Loyal Customers', and 'Champions' based on their CLV.
- **Segment Analysis**: Groups customers to understand the average spending behavior within each segment.

## Dependencies
- `lifetimes`: A Python library for CLV calculations.
- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `matplotlib` and `seaborn`: For data visualization.

The script uses synthetic grocery data sourced from a GitHub repository.

## Usage
Ensure you have the necessary libraries installed using `pip install lifetimes`. Run the script with Python 3, and it will output the segmented customer data along with predictive CLV values.

## Contributions
The script was a collaborative effort by Alberto Diaz, Laura Cepero Navarro, and Orialys Ruiz.

## License
The details of the license can be added here based on the usage and sharing rights you want to enforce.
