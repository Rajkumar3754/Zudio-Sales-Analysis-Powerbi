# Zudio Sales Analysis 2024📊



## ✨ Overview

The **Zudio Sales Analysis 2024** project is a powerful tool designed to analyze sales data for Zudio in the year 2024. This project uses a combination of **Power BI**, **SQL**, **Excel**, and **Oracle Database** to manage, analyze, and visualize sales data. The goal is to help Zudio gain deep insights into their sales performance across various products, categories, regions, and time periods to make data-driven decisions for better inventory management, marketing strategies, and business growth.

---

## 🚀 Technologies Used

- **Power BI**: For creating dynamic, interactive visualizations and reports.
- **SQL**: For querying and managing data in the relational database.
- **Oracle Database**: For handling large datasets and performing complex queries.
- **Excel**: For importing and cleaning raw sales data.
- **Power BI Desktop**: For building and testing reports before publishing.
- **Power BI Service**: For sharing reports online with stakeholders.

---

## 💡 Features

### 🔎 Product & Profit Analysis
- Analyze sales data to understand which products are top performers.
- Breakdown of **total sales**, **profit margins**, and **quantity sold** for each product.
- Insights into the most and least profitable products, helping to identify inventory and marketing priorities.

### 🌍 Geographical Insights
- Visualize sales performance across different regions (city, state, country).
- Understand regional trends in product popularity, assisting with targeted marketing and distribution strategies.

### 📅 Time-Based Sales Trends
- Track sales performance over time—monthly, quarterly, and annually.
- Identify peak sales periods and seasonal trends, which are crucial for forecasting and resource allocation.

### 📊 Interactive Dashboards
- Create dynamic dashboards with **filters** for in-depth exploration of data by:
  - Product category (e.g., Men, Women, Kids)
  - Geographic location (City, State, Country)
  - Time period (Year, Quarter, Month)
  
### 📈 KPI Tracking
- Display essential **Key Performance Indicators (KPIs)** such as **Total Sales**, **Total Profit**, and **Total Quantity Sold** to track overall business health.

---

## 🔄 Data Flow

### 1. **Data Import**
   - Raw **Excel** files containing sales data are imported into the **SQL database** using an automated ETL (Extract, Transform, Load) process.
   - The data includes key columns such as: Product Name, Sales Amount, Profit, Category, Clothing Type, Quantity Sold, City, State, and Country.

### 2. **Data Transformation**
   - Clean and preprocess the data using **SQL**:
     - Handle missing values (e.g., NULL or NaN values).
     - Remove duplicate records.
     - Standardize formats for currency, dates, and numerical values.

### 3. **Power BI Visualization**
   - Import the cleaned and aggregated data into **Power BI** for visualization.
   - Build **interactive dashboards** showcasing key insights such as:
     - **Sales trends** over time.
     - **Top-selling products** and their performance.
     - **Sales by geographical region** using map visualizations.
     - **KPI indicators** like total sales and total profit.

---

## 🛠️ How to Set Up

### Requirements

- **Microsoft Excel**: For importing raw sales data.
- **Power BI Desktop**: For creating, testing, and publishing interactive reports and dashboards.
- **SQL Database (MySQL, Oracle)**: For storing and querying sales data.
- **Power BI Service** (Optional): For publishing reports online for stakeholders.

### Setup Instructions

#### 1. **Prepare the Data**
   - Collect **Excel** files containing sales data for 2024. Ensure the data includes:
     - Product Name
     - Category (Men, Women, Kids, etc.)
     - Clothing Type
     - Sales Amount
     - Profit
     - Quantity Sold
     - City, State, Country
     - Order Date (Time)

#### 2. **Create Database and Import Data**
   - Open your **SQL** database (MySQL or Oracle).
   - Create a table `sales_data` to store the imported data.

   - Import your Excel data into the `sales_data` table using an appropriate import tool (e.g., SQL Server Management Studio, MySQL Workbench).

#### 3. **Power BI Integration**
   - Open **Power BI Desktop** and click on **Get Data** to import data from **SQL Server** or **Excel**.
   
     Steps to import from SQL:
   - Go to **Home** > **Get Data** > **SQL Server**.
   - In the **SQL Server database** dialog, enter the server and database name.
   - Choose the authentication method and credentials.
   - Click **OK** to connect and choose the **sales_data** table.

     Steps to import from Excel:
   - Go to **Home** > **Get Data** > **Excel**.
   - Browse to select the Excel file and click **Open**.
   - Choose the worksheet containing the sales data and click **Load**.

#### 4. **Data Transformation in Power BI (Optional)**
   - After loading the data, use **Power Query** in Power BI to clean and transform the data:
     - Remove unnecessary columns.
     - Replace missing or null values with zeros or appropriate values.
     - Standardize data formats (e.g., dates, currency).
   - To open **Power Query**, click on **Transform Data** after loading the data.

#### 5. **Building Visualizations in Power BI**

   - Start creating your visualizations using the drag-and-drop interface in **Power BI Desktop**:
     - **Bar Charts**: Drag **Product Name** to the axis and **Total Sales** to the value to visualize product performance.
     - **Pie Charts**: Drag **Category** to the legend and **Total Sales** to the values for category-wise breakdowns.
     - **Line Charts**: Drag **Order Time** (Date) to the axis and **Total Sales** to the values to visualize sales trends over time.
     - **Map Visualizations**: Drag **City** or **Region** to the location and **Total Sales** to the size for geographical distribution of sales.
     - **KPI Cards**: Drag **Total Sales** and **Profit** into a card visualization to display KPIs.

#### 6. **Add Interactivity with Slicers**
   - Slicers allow you to filter data dynamically. To add a slicer:
     - From the visualizations pane, select **Slicer**.
     - Drag the desired field (e.g., **Category**, **City**, or **Order Time**) into the slicer.
     - Users can click on the slicer values to filter the entire report by selected categories.

#### 7. **Save and Publish Your Report**
   - Save your report by clicking **File** > **Save As**.
   - To publish to Power BI Service:
     - Go to **Home** > **Publish**.
     - Choose the workspace in Power BI Service where you want to publish the report.
   
  Once published, stakeholders can access the reports from **Power BI Service**.


