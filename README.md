# Sales Data Analysis Project

## Project Overview

This project explores sales data using **Python, Pandas, NumPy, and Matplotlib** to understand business performance and identify useful insights.

The analysis focuses on sales revenue, product categories, regional performance, sales channels, payment methods, and customer types. The goal is to transform raw sales data into meaningful information that can support better business decisions.

## Dataset

The dataset contains **1,000 rows and 14 columns**.

Key columns include:

- `Product_ID`: Product identifier
- `Sale_Date`: Date of the transaction
- `Sales_Rep`: Sales representative
- `Region`: Sales region
- `Sales_Amount`: Recorded sales amount
- `Quantity_Sold`: Number of units sold
- `Product_Category`: Product category
- `Unit_Cost`: Cost per unit
- `Unit_Price`: Selling price per unit
- `Customer_Type`: New or Returning customer
- `Discount`: Discount applied
- `Payment_Method`: Payment method used
- `Sales_Channel`: Online or Retail

## Tools and Technologies

- **Python** – Data analysis
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Jupyter Notebook** – Development environment

## Project Steps

### 1. Data Loading and Exploration
- Imported the dataset using Pandas.
- Explored the first rows using `head()`.
- Checked dataset dimensions and column types.
- Reviewed descriptive statistics.

### 2. Data Cleaning
- Checked for missing values.
- Checked for duplicated records.
- Examined numerical values for negative amounts.
- Checked whether discounts were within the expected range.

### 3. Sales Performance Analysis
- Calculated total revenue, cost, profit, and profit margin using quantity and unit price/cost.
- Explored the distribution of sales.
- Examined monthly sales performance.

### 4. Product and Regional Analysis
- Compared sales across product categories.
- Analyzed sales performance across regions.
- Used a pivot table to compare product categories by region.

### 5. Sales Representative Analysis
- Explored sales performance by representative.
- Compared contributions across sales representatives.

### 6. Customer Analysis
- Compared New and Returning customer transactions.
- Examined revenue and transaction patterns by customer type.

### 7. Sales Channel and Payment Analysis
- Compared Online and Retail sales.
- Examined the popularity of different payment methods.
- Compared transaction counts and recorded sales amounts.

### 8. Correlation and Relationships
- Planned to examine relationships between numerical variables.
- Explore correlations involving sales amount, quantity sold, discount, unit cost, and unit price.

## Key Findings

Some observations from the analysis:

- The dataset contains 1,000 transactions with no missing values or duplicated rows in the initial checks.
- Retail recorded 512 transactions, compared with 488 for Online.
- Retail recorded approximately 2.56 million in `Sales_Amount`, while Online recorded approximately 2.46 million.
- Cash was the least-used payment method, with 313 transactions.
- The North region recorded the highest sales amount in Clothing, Electronics, and Furniture.
- The East region recorded the highest sales amount in Food.

## Data Quality Considerations

One important issue requires further investigation: the total of `Sales_Amount` differs significantly from the total calculated using `Quantity_Sold * Unit_Price`.

For this reason, `Sales_Amount` is used as the recorded sales measure in the channel and regional comparisons. Revenue, cost, and profit calculations based on unit price and quantity should be validated before being treated as final business results.

## How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib jupyter
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the sales analysis notebook.
5. Make sure the dataset path in the notebook points to the correct CSV file.
6. Run the notebook cells in order.



## Conclusion

This project demonstrates the use of Python for exploratory data analysis and business performance evaluation. It provides an opportunity to practice data cleaning, data manipulation, visualization, and business interpretation while identifying areas that require further investigation.

---

**Author:** Zouhair 
**Project:** Sales Data Analysis  
**Tools:** Python | Pandas | NumPy | Matplotlib | Jupyter Notebook
