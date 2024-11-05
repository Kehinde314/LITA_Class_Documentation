# LITA_Class_Documentation

### Project Title: Capstone Project

### Project Overview 
This Data Analysis project aims to generate insights found in Excel, SQL, and PowerBi which includes a sales overview, top-performing products, and regional breakdowns.

### Data Sources
The primary source of Data used here is "so the maximum number of rolls.csv"

### Tools Used
- Microsoft Excel [Download Here](https://www.microsoft.com/en-us/microsoft-365/p/excel/cfq7ttc0k7dx)
- SQL Structural Query Language
- PowerBi for Data Visualization
- GitHub for portfolio making

### Data Analysis
This is where we include some of the DAX expressions used during our analysis

```SQL
CREATE TABLE Sales (
    SN INT IDENTITY(40,40) PRIMARY KEY, -- Auto-incrementing serial number starting from 1
    Transaction_ID INT NOT NULL,
    Product_ID VARCHAR(10) NOT NULL,
    Product_Name VARCHAR(50) NOT NULL,
    Quantity INT NOT NULL,
    Revenue DECIMAL(10, 2) NOT NULL,
    Date DATE NOT NULL,
    Region VARCHAR(50),
    Store_ID VARCHAR(10),
    Customer_ID VARCHAR(10),
    Transaction_Category VARCHAR(20)
);
```
