# Market Basket Analysis for Allias Megastore

## Project Overview
This project focuses on conducting a market basket analysis for Allias Megastore, a large international retail store, using real transactional sales data. The goal is to identify associations between products frequently bought together to provide valuable business insights for more effective product bundling and marketing strategies.

## Dataset
The dataset includes the following key columns:
- **OrderID**: Unique identifier for each sales order.
- **CustomerID**: Unique identifier for each customer.
- **ProductName**: Name of the product purchased.
- **Quantity**: Quantity of the product sold.
- **InvoiceDate**: Date of the transaction.
- **UnitPrice**: Price per unit of the product.
- **TotalCost**: Total cost of the transaction.
- **Country**: Country of the customer.
- **Order Priority**: Priority level of the order.
- **Region**: Geographic region of the customer.
- **Segment**: Market segment of the customer.
- **PaymentMethod**: Method of payment used.
- **CustomerRewardsMember**: Whether the customer is a rewards program member.

## Goals of Analysis
- To identify associations between products purchased together using the **Apriori algorithm**.
- To uncover patterns and trends in the transactional data that can inform product bundling strategies and marketing campaigns.
- Provide actionable insights that will help improve profits by better targeting customers.

## Key Steps
1. **Data Cleaning and Preparation**:
   - Categorical variables were selected and encoded using appropriate methods.
   - The dataset was transactionalized to suit market basket analysis.
   
2. **Running Apriori Algorithm**:
   - The **Apriori algorithm** was applied to the transactional data to generate frequent itemsets.
   - Association rules were extracted from these frequent itemsets, with metrics like support, confidence, and lift calculated.

3. **Top Association Rules**:
   - The top 3 rules were identified and analyzed to uncover the strongest product associations.

## Project Files
- **megastore_dataset.csv**: The original dataset used for the analysis.
- **Market_Basket_Analysis.ipynb**: Jupyter notebook containing the code for the entire process, including data cleaning, preparation, and Apriori algorithm implementation.
- **top_3_rules.csv**: CSV file containing the top 3 association rules.
- **README.md**: This document explaining the project.

## How to Run
To run the analysis on your local machine:
1. Clone the repository.
2. Install the necessary libraries:
   ```bash
   pip install pandas scikit-learn mlxtend
   ```
3. Open the Jupyter notebook `Market_Basket_Analysis.ipynb` and run all cells to reproduce the analysis.

## Key Libraries Used
- **pandas**: For data manipulation and cleaning.
- **scikit-learn**: For encoding categorical variables.
- **mlxtend**: For the Apriori algorithm and generating association rules.

## Results
The analysis revealed key product associations, such as:
- **SET6 RED SPOTTY PAPER PLATES** and **SET6 RED SPOTTY PAPER CUPS** often being bought together.
- Products in the same category tend to have a high lift and confidence, indicating strong product bundling potential.

## Conclusion
The results of this analysis provide valuable insights for Allias Megastore, helping them better understand customer purchase behavior and optimize their marketing strategies by creating targeted product bundles based on frequently bought together items.
