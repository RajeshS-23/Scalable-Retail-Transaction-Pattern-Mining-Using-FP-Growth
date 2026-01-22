# Market Basket Analysis Using FP-Growth Algorithm

## Overview
This project performs Market Basket Analysis to identify frequently purchased item combinations from retail transaction data.  
The FP-Growth algorithm is used to efficiently mine frequent itemsets without generating candidate itemsets, making it faster than traditional Apriori for large datasets.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- mlxtend

---

## Dataset
- File name: `Market_Basket_Optimisation.csv`
- Each row represents a customer transaction
- Each column represents an item
- Missing values indicate that an item was not purchased in a transaction

---

## Project Workflow

1. Load the transaction dataset
2. Perform basic data exploration
3. Convert transactions into a one-hot encoded format using `TransactionEncoder`
4. Apply the FP-Growth algorithm to mine frequent itemsets
5. Analyze frequent itemsets based on minimum support

---

## Data Preprocessing
- Transaction data is converted into boolean (True/False) format
- One-hot encoded representation is required for FP-Growth
- No manual handling of missing values is needed

---

## FP-Growth Algorithm
- Minimum Support: `0.001`
- Uses a tree-based approach for efficient frequent pattern mining
- Faster and more scalable than Apriori for large datasets

---

## Output
The output is a DataFrame containing:
- Frequent itemsets
- Support values for each itemset

These results can be used for further association rule generation.

---

## Use Cases
- Product recommendation systems
- Retail analytics
- Customer purchase pattern analysis
- Inventory planning

---

## How to Run the Project

1. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib mlxtend
