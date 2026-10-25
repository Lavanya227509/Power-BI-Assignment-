📊 Sales Data Preparation & Modelling

A Power BI - Power Query Project
Transforming raw order data into structured, analysis-ready information.
Power BI Desktop - Power Query Editor - Power Query M - Data Cleaning - Data Modelling

📌 Project Overview
This project documents a sales-data preparation workflow in Microsoft Power BI. It brings together transformations covering data types, text formatting, derived columns, conditional logic, merging.
Documentation basis: the supplied seven-page project PDF.

🎯 Project Objectives
- Organize order and transaction data for analysis.
- Standardize text fields and assign appropriate data types.
- Create Location, Profit Margin, and Profit Status fields.
- Review missing values and duplicate records.
- Combine related data and prepare summary tables.
- Document the Power BI model and summary outputs.

🧰 Tools & Technologies
- **Power BI Desktop:** For data modelling, relationship creation and report building.
- **Power Query Editor (M Language):** For data cleaning, transformation.
    - Text.Transform, Text.Proper for standardizing text
    - Table.Group for Grouping (Your Grouping Table: Order_Id_Count, Avg_Profit_Category)
    - Merge Queries for combining Orders + Sales Target tables
- **DAX:** 
    - Profit Margin = DIVIDE([Profit], [Amount])
    - Profit Status = IF([Profit Margin] > 0, "Profit", "Loss")
    - Location = [City] & ", " & [State]
- **Data Cleaning:** Remove Duplicates, Replace Values, Fill Down for missing values
- **Data Modelling:** Creating relationships between Order Details, List of Orders, Sales Target
- **Visuals:** Card (332 Orders, 15.97 Avg Profit), Table (Category-wise profit)

📁 Files
- Power BI Assignment 1 Lav.pbix
- README.md
