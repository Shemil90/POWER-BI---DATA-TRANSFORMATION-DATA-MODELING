# POWER-BI---DATA-TRANSFORMATION-DATA-MODELING

📌 Project Overview

This assignment focuses on practical data transformation, data cleaning, data merging, aggregation, and data modeling using Microsoft Power BI.

The objective is to transform raw CSV datasets into structured and analysis-ready data by applying Power Query operations, creating calculated columns, handling missing and duplicate data, and establishing relationships between multiple tables.

🎯 Objectives

- Import multiple CSV datasets into Power BI.
- Perform data cleaning and transformation using Power Query Editor.
- Create custom and conditional columns.
- Merge datasets using appropriate join conditions.
- Identify and handle missing values and duplicate records.
- Apply sorting and filtering techniques.
- Perform grouping and aggregation operations.
- Establish relationships between tables to build a structured data model.

🛠️ Tools & Technologies

- Microsoft Power BI Desktop
- Power Query Editor
- Data Transformation
- Data Modeling
- Data Merging and Relationships

📂 Datasets Used

The assignment uses the following three datasets:

1. List of Orders.csv – Contains order-related information.
2. Order Details.csv – Contains order details, including category, sub-category, amount, and profit.
3. Sales Target.csv – Contains sales target information.

📊 Tasks Performed

1. Data Import

- Imported "List of Orders.csv" into Power BI.
- Opened Power Query Editor using the Transform option.
- Imported "Order Details.csv" and "Sales Target.csv".

2. Data Transformation

Performed the following transformations using Power Query Editor:

- Restricted the "List of Orders" table to the first 500 rows.

- Changed the "Order Date" column data type to Date.

- Changed "Amount" and "Target" columns to Fixed Decimal Number.

- Converted the "CustomerName" column into Proper Case.

- Merged "State" and "City" columns to create a new "Location" column in the format "City, State".

- Created a custom column named "Profit Margin" using the formula:
  
  "Profit Margin = (Profit / Amount) × 100"

- Created a conditional column named "Profit Status" based on profit values:
  
  - Loss: Profit less than 0.
  - Break-Even: Profit equal to 0.
  - Profit: Profit greater than 0.

3. Data Merging (Joins)

- Merged "List of Orders" and "Order Details" using the "Order ID" column.
- Created a new combined table named Orders Data.
- Used the Order ID relationship to connect order information with detailed sales information.

4. Handling Missing Values & Duplicates

- Identified missing or null values across the datasets.
- Evaluated appropriate strategies for handling missing values.
- Checked datasets for duplicate records.
- Considered removing duplicate records where appropriate to maintain data accuracy and consistency.

5. Sorting and Filtering

Applied sorting and filtering techniques to analyze the data:

- Sorted orders by "Order Date" in descending order to identify recent orders.
- Filtered records based on a specific state, such as Tamil Nadu, for regional analysis.
- Used columns such as State and Category to explore relevant subsets of data.

6. Grouping and Aggregation

Order Details Table:

- Duplicated the "Order Details" table.
- Calculated the count of each Order ID.
- Calculated average profit by Category.
- Calculated total Amount by Sub-Category.

Sales Target Table:

- Duplicated the "Sales Target" table.
- Aggregated the total Target Amount by Month of Order Date.

7. Data Modeling

Established relationships between tables using Power BI's Manage Relationships feature:

- Created a relationship between "List of Orders" and "Order Details" using "Order ID".
- Created a relationship between "Order Details" and "Sales Target" using "Category".
- Checked relationship settings and ensured the specified relationships were active.
