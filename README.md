# Online Retail Data Cleaning

## Overview

This project focuses on cleaning, preprocessing, and analyzing a large-scale retail transaction dataset containing over 1 million records. The dataset includes real-world issues such as missing values, duplicate records, cancelled orders, negative quantities, invalid prices, and outliers.

The objective of this project is to demonstrate practical Data Analytics and Data Cleaning techniques using Python, Pandas, NumPy, Matplotlib, and Seaborn in Google Colab.

---

## Dataset Information

**Dataset:** Online Retail II (UCI Machine Learning Repository)

**Size:**

* Rows: 1,067,371
* Columns: 8

### Features

| Column      | Description                |
| ----------- | -------------------------- |
| Invoice     | Invoice Number             |
| StockCode   | Product Code               |
| Description | Product Description        |
| Quantity    | Quantity Purchased         |
| InvoiceDate | Transaction Date           |
| Price       | Unit Price                 |
| Customer ID | Unique Customer Identifier |
| Country     | Customer Country           |

---

## Project Objectives

* Perform comprehensive data cleaning
* Handle missing values
* Remove duplicate records
* Filter cancelled transactions
* Remove invalid quantities and prices
* Convert date columns into proper datetime format
* Create new analytical features
* Detect and handle outliers
* Perform exploratory data analysis (EDA)
* Generate business insights from retail transactions

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## Data Cleaning Process

### 1. Missing Value Treatment

Identified missing values in:

* Customer ID
* Description

Actions taken:

* Removed records with missing Customer IDs
* Replaced missing product descriptions with "Unknown Product"

---

### 2. Duplicate Removal

Removed exact duplicate records to improve data quality and avoid biased analysis.

---

### 3. Cancellation Handling

Invoices beginning with the letter **"C"** were identified as cancelled transactions and removed from the dataset.

---

### 4. Invalid Quantity Removal

Removed transactions with:

* Zero quantity
* Negative quantity

These records generally represent returns or incorrect entries.

---

### 5. Invalid Price Removal

Removed transactions with:

* Zero price
* Negative price

These values may indicate refunds, promotional items, or data entry errors.

---

### 6. Date Conversion

Converted the InvoiceDate column into datetime format to enable time-series analysis.

---

### 7. Feature Engineering

Created a new column:

```python
Revenue = Quantity × Price
```

This metric is used for sales analysis and business insights.

---

### 8. Outlier Detection

Applied the Interquartile Range (IQR) method to identify and remove extreme values from:

* Quantity
* Price

This improves visualization quality and analytical accuracy.

---

## Exploratory Data Analysis

The project includes analysis such as:

* Revenue Distribution
* Monthly Sales Trends
* Top Selling Products
* Top Revenue Generating Countries
* Customer Purchase Patterns
* Product Performance Analysis

---

## Key Business Insights

Examples of insights generated:

* Highest revenue-generating products
* Countries contributing the most sales
* Monthly revenue trends
* Customer purchasing behavior
* Sales distribution patterns

---

## Project Structure

```text
├── Agentic_AI_Internship_Online_Retail.ipynb
├── Cleaned_Online_Retail.csv
├── README.md
└── Dataset
    └── online_retail_II.csv
```

---

## How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/online-retail-data-cleaning.git
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

### Run Notebook

Open:

```text
Agentic_AI_Internship_Online_Retail.ipynb
```

in:

* Google Colab
* Jupyter Notebook

and execute all cells.

---

## Learning Outcomes

Through this project, I gained practical experience in:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis
* Feature Engineering
* Outlier Detection
* Data Visualization
* Business Insight Generation
* Python for Data Analytics

---

## Future Enhancements

* Customer Segmentation using RFM Analysis
* Predictive Sales Forecasting
* Customer Lifetime Value Analysis
* Interactive Dashboard using Power BI/Tableau
* Machine Learning Models for Customer Behavior Prediction

---

## Author

**Tanay G**

B.Tech Computer Science Engineering Student

Passionate about Data Analytics, Artificial Intelligence, Software Development, and Problem Solving.

---

## License

This project is intended for educational and portfolio purposes.
# Data-Cleaning-using-Pandas
