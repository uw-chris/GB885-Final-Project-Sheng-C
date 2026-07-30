**RUSH Sales Analysis — Python Final Project**

**Overview**
Analysis of RUSH sportswear/footwear sales data (2020–2021) on behalf of the VP of US Sales. The raw data was provided as three separate tables (sales transactions, retailer locations, and product categories) and required cleaning before analysis.
Business Questions Answered
1. Which product category had the highest dollar sales in 2021?
2. Which state had the highest dollar sales of women's products in 2021?
3. Which state had the highest dollar sales of men's products in 2021?
4. Which retailer purchased the most units in 2021? In 2020?

**Repository Structure**
├── README.md
├── .gitignore
├── RUSH_Analysis.ipynb        # main analysis notebook
└── data/
    ├── TABLE_SALES_885.csv
    ├── TABLE_RETAILER_885.csv
    └── TABLE_PRODUCTS_885.csv

**Data Sources**
* TABLE_SALES — order-level transactions (date, product, price, units, sales method)
* TABLE_RETAILER — retailer name and location by retailer ID
* TABLE_PRODUCTS — product category names by product ID
Field definitions are documented in the accompanying data dictionary.

**Data Cleaning Notes**
The raw data contained several issues that were identified and resolved (see notebook Section 2 for details):
* Non-numeric placeholder values in the units-sold field
* A small number of missing and clearly invalid price values
* A misspelled category label in the sales-method field
* One transaction referencing a retailer ID not present in the retailer table

**How to Run**
Open RUSH_Analysis.ipynb in Google Colab or Jupyter. The notebook loads the CSVs from the data/ folder using relative paths, so it will run end-to-end without any setup as long as the repo structure above is preserved.
