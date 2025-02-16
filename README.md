# Market-Basket-Analysis-Using-Apriori-Algorithm

**Overview**
This project applies the Apriori algorithm to perform market basket analysis on retail transaction data. The dataset is sourced from the UCI Machine Learning Repository and contains online retail transactions. The goal is to uncover frequent itemsets and association rules that help identify product relationships, aiding in better inventory control and marketing strategies.

**Dataset**
The dataset is obtained from UCI's Online Retail database, consisting of transaction records including:

InvoiceNo – Unique identifier for each transaction
Description – Product name
Quantity – Number of items purchased
Country – Location of the transaction


**Steps in the Analysis**
**1. Data Preprocessing**
Load the dataset and remove missing values.
Exclude canceled transactions (marked with 'C' in InvoiceNo).
Subset the dataset by country (United Kingdom and Ireland).
**2. Data Transformation**
Convert transaction data into a one-hot encoded matrix.
Ensure each transaction contains at least two items to perform meaningful analysis.
**3. Frequent Itemset Mining**
Use the Apriori algorithm to extract frequent itemsets based on a minimum support threshold.
Compute itemset length to analyze the size of common item combinations.
**4. Association Rule Generation**
Apply the Association Rules Algorithm to generate rules based on lift, confidence, and support.
Different confidence thresholds are used for UK (0.7) and Ireland (0.95) due to differences in transaction volume.
Key Findings

**United Kingdom:** Higher transaction volume led to more robust association rules with significant lift values.
Ireland: Lower transaction volume required a higher confidence threshold to extract meaningful rules.
Popular items such as teacups and saucers showed strong association patterns, indicating customer preferences.

**Technologies Used**
Python
Pandas (for data manipulation)
Mlxtend (for Apriori algorithm and association rules)
Usage

**Results & Insights**   
   
The extracted association rules help businesses:
      ->Optimize inventory management.
      ->Create bundle offers based on frequently purchased items.
      ->Improve product placement strategies.
