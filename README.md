# Nashville Housing Data Cleaning and Transformation
![image](https://github.com/user-attachments/assets/aa91c4d7-537e-42f2-baed-f860aa4a932d)

https://public.tableau.com/app/profile/amir2848/viz/GMC_Checkpoint/Dashboard1

## Project Overview
This project demonstrates how to transform raw data from a Nashville housing dataset into structured, usable information using SQL. The primary focus is on comprehensive data cleaning, standardization, and preparation, covering tasks essential for real-world data analysis projects. This includes dealing with inconsistent data formats, populating missing values, breaking down complex columns, and removing duplicates.

---

## Project Steps

### 1. Importing the Data
- **Data Setup**: The project starts by importing the raw Nashville housing data into a SQL Server database.
- **ETL Introduction**: Briefly discusses the Extract, Transform, Load (ETL) process, emphasizing data transformation as a critical step before analysis.

---

## Data Cleaning and Transformation

### 2. Standardizing Date Formats
- **Objective**: Clean the "Sale Date" column, which initially includes both date and time.
- **Solution**: Use the `CONVERT` function to extract just the date portion, resulting in a cleaner and more practical format.
- **Example Code**:
  ```sql
  SELECT CONVERT(date, [Sale Date]) AS SaleDate
  FROM NashvilleHousingData;
