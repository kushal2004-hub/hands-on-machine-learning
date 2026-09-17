## 🛒 E-Commerce Data Cleaning & Exploratory Data Analysis


## 📌 Project Overview
This notebook performs comprehensive data cleaning and exploratory analysis on an e-commerce dataset containing customer orders and order details. The goal is to prepare raw data for further analysis or machine learning tasks by handling missing values, fixing inconsistencies, and visualizing key patterns.

## 📂 Dataset Description
1. Orders Dataset (List of Orders.csv)
Contains customer order information:

Order ID: Unique identifier for each order

Order Date: Date when order was placed (DD-MM-YYYY)

CustomerName: Name of the customer

State: State where order was delivered

City: City where order was delivered

2. Order Details Dataset (Order Details.csv)
Contains product-level order information:

Order ID: Links to Orders dataset

Amount: Total amount for the product

Profit: Profit/Loss on the product

Quantity: Number of units ordered

Category: Product category (Furniture, Clothing, Electronics)

Sub-Category: Specific product sub-category

## 🔧 Data Cleaning Steps Performed

Step	Operation	Description
1	File Upload	Used google.colab.files.upload() to load CSV files
2	Initial Inspection	head(), tail() to understand data structure
3	Duplicate Check	duplicated().sum() - Found 0 duplicates ✅
4	Missing Value Handling	fillna('').astype(str) to handle NaN before string operations
5	String Standardization	.str.title().str.strip() to clean text fields
6	Data Replacement	Fixed misspellings: 'Deli' → 'Delhi', 'Hankerchief' → 'Handkerchief'
7	Category Fixes	Corrected 'Furniure' → 'Furniture', 'Clotcing' → 'Clothing'
8	Drop Missing Values	dropna() to remove rows with null values

## 📊 Exploratory Data Analysis

Categorical Analysis
Unique Cities: 24 cities across India

Unique Categories: 3 main categories (Furniture, Clothing, Electronics)

Unique Sub-Categories: 17 different product types

Outlier Detection (Box Plots)
Amount: Identified high-value outliers > 4000

Profit: Both positive and negative outliers (range: -1981 to 1864)

Quantity: Outliers up to 14 items per order

## 📈 Key Insights

✅ No duplicate records found in either dataset

✅ Fixed misspelled city names (e.g., 'Deli' → 'Delhi')

✅ Corrected category inconsistencies ('Furniure' → 'Furniture')

✅ Removed invalid payment method ('share transfer')

✅ Identified significant outliers in Amount, Profit, and Quantity columns

✅ 24 unique cities across 19 states in India

## 🛠️ Technologies Used
Library	Purpose
Pandas	Data manipulation and cleaning
NumPy	Numerical operations
Matplotlib	Basic plotting and visualizations
Seaborn	Statistical data visualization
Plotly	Interactive charts (imported but not used)

## 🚀 How to Run
Open in Google Colab

Run the first cell to install required libraries

When prompted, upload List of Orders.csv and Order Details.csv

Run all cells sequentially

View the cleaned data and box plots at the end

## 🎯 Learning Outcomes
✅ Handling file uploads in Google Colab

✅ Data cleaning techniques with Pandas

✅ Handling missing values (NaN) in string columns

✅ Fixing inconsistent categorical data

✅ Outlier detection using box plots

✅ Data visualization best practices