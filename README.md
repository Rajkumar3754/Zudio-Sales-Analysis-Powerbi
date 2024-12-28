# Zudio Sales Analysis 2024



## ✨ Overview

The **Zudio Sales Analysis 2024** project provides a comprehensive analysis of Zudio's sales data for the year 2024. This project is built using **Power BI** for data visualization, **SQL** for data management, and **Excel** as the data input. It allows Zudio to track performance across various products, categories, and geographical locations, enabling the business to make informed decisions regarding inventory, marketing, and future growth strategies.

---

## 🚀 Technologies Used

- **Power BI**: For creating dynamic visualizations and reports.
- **SQL**: Used for querying and managing sales data in the database.
- **Oracle Database**: For handling larger datasets and complex queries.
- **Excel**: For importing raw data into the system.

---

## 💡 Features

### 🔎 Product & Profit Analysis
- Breakdown of total sales, profit margins, and quantity sold for each product.
- Identify top-performing products and their profitability.

### 🌍 Geographical Insights
- Visualize sales performance across different regions (city, state, country).
- Identify trends and differences in product popularity across regions.

### 📅 Time-Based Sales Trends
- Track and visualize sales trends over time: monthly, quarterly, and annually.
- Identify peak sales periods and seasonal trends.

### 📊 Interactive Dashboards
- Create interactive filters in Power BI for in-depth exploration of sales data by:
  - Product category
  - City, state, or country
  - Time period

---

## 🔄 Data Flow

1. **Data Import**
   - Import raw **Excel** data into the **SQL database** using an automated process.
   - Data columns include: Product Name, Total Sales, Profit, Category, Clothing Type, Quantity Sold, City, State, and Country.

2. **Data Transformation**
   - Clean and preprocess data in SQL:
     - Handle missing values
     - Remove duplicates
     - Standardize formats (currency, dates, etc.)

3. **SQL Queries**
   - Aggregate data using SQL queries to get key metrics:
     ```sql
     SELECT product_name, SUM(total_sales) AS total_sales, SUM(profit) AS total_profit
     FROM sales_data
     GROUP BY product_name;
     ```

4. **Power BI Visualization**
   - Import the processed data into Power BI.
   - Build interactive dashboards showcasing:
     - Sales trends over time.
     - Top-selling products.
     - Sales by geographical region.

---

## 🛠️ How to Set Up

### Requirements

- **Microsoft Excel**: For handling the raw data.
- **Power BI**: For building the interactive reports and dashboards.
- **SQL Database (MySQL or Oracle)**: For managing and querying the sales data.
- **Power BI Desktop**: For visualization.

### Setup Instructions

1. **Prepare the Data**  
   - Gather **Excel** files containing sales data.
   - Ensure data contains columns such as: Product Name, Category, Sales Amount, Profit, and Geographical information (City, State, Country).

2. **Import Data into SQL Database**  
   - Open your SQL database (e.g., MySQL or Oracle).
   - Create a table named `sales_data` and import the Excel data into this table.
   
   Example SQL query to create the table:
   ```sql
   CREATE TABLE sales_data (
       product_name VARCHAR(255),
       total_sales DECIMAL(10,2),
       profit DECIMAL(10,2),
       category VARCHAR(100),
       clothing_type VARCHAR(100),
       order_time DATETIME,
       quantity INT,
       total_cost DECIMAL(10,2),
       city VARCHAR(100),
       state VARCHAR(100),
       country VARCHAR(100)
   );
