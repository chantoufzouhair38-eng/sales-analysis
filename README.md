Sales Analysis with Python

Exploratory analysis of a sales dataset (1,000 transactions) using pandas, NumPy and matplotlib. The goal is to understand which products, regions, sales reps and sales conditions drive revenue.

Dataset
File: DATA/sales.csv
Size: 1,000 rows, 14 columns
Main columns: Sale_Date, Sales_Rep, Region, Product_Category, Sales_Amount, Quantity_Sold, Unit_Cost, Unit_Price, Discount, Customer_Type, Payment_Method, Sales_Channel
Data quality: no missing values, no duplicates, no negative values
Questions explored
Which sales reps and product categories perform best?
How do sales change from month to month?
Do customer type, payment method or sales channel make a difference?
How does the discount level relate to revenue?
Which region leads in each product category?
Key findings
Top sales rep: David generates the most revenue (about 1.14M), but Bob has the highest average sale.
Top category: Clothing is the highest-revenue category (about 1.31M).
Seasonality: January has the highest monthly revenue (about 495K). A higher quantity sold does not always mean higher revenue.
Customer type and sales channel: New vs returning customers and online vs retail show almost no difference.
Payment method: Cash is the least used method, but the gap with the others is small.
Best region per category: North leads in Clothing, Electronics and Furniture; East leads in Food.
Limitations and next steps
Sales_Amount does not match Quantity_Sold × Unit_Price × (1 − Discount), so revenue and profit depend on which column is used. This needs to be clarified before drawing profit conclusions.
The profit margin should be recalculated with the discount applied.
The discount analysis should use discount bands (for example 0–10%, 10–20%, 20–30%) instead of exact values.
Statistical tests could confirm whether the small differences between groups are real or just noise.
Project structure
sales-analysis/
├── README.md
├── notebooks/
│   └── sales_analysis.ipynb
├── DATA/
│   └── sales.csv
├── graphes/            # saved charts
└── .gitignore
How to run
bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/sales-analysis.git
cd sales-analysis

# 2. Install the dependencies
pip install pandas numpy matplotlib jupyter

# 3. Open the notebook
jupyter notebook notebooks/sales_analysis.ipynb
Tools

Python · pandas · NumPy · matplotlib · Jupyter Notebook

Author

Zouhair — Computer Science student, learning data analysis.
