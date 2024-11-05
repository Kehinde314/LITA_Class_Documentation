# LITA_Class_Documentation

### Project Title: Capstone Project

[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Tools Used](#tools-used)

[Data Analysis](#data-analysis)

[Data Visualization](#data-visualization)

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

Here is another expression used to insert data into the table

```SQL
BULK INSERT Sales
FROM 'C:\Users\Admin\OneDrive\??\so the maximum number of rolls.csv'
WITH (
    FIELDTERMINATOR = ',', 
    ROWTERMINATOR = '\n',
    FIRSTROW = 2 -- Skip header row if present
);
```

### Data Visualization
---
![so the maximum number of rolls csv](https://github.com/user-attachments/assets/4dbb8574-a144-47c0-8dac-b46abe20db0e)

![Microsoft SQL Server Management Studio](https://github.com/user-attachments/assets/db97f575-4ea4-4b68-afdc-65c70a2ae0ac)

![Power BI Desktop](https://github.com/user-attachments/assets/08b092b9-a608-467c-bd8a-070cec08e191)


