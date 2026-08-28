# 📊 Sales & Customer Analytics Dashboard (Power BI)

## 🎯 Project Overview
This project is a comprehensive, end-to-end Power BI dashboard designed to provide actionable insights into sales performance, product profitability, and customer behavior. The objective was to transform raw, fragmented regional data into a centralized, interactive data model that drives business decisions.

---

## 🛠️ 1. Data Engineering & ETL (Power Query)
The raw data was extracted from multiple sources and underwent rigorous cleaning and transformation using **Power Query Editor**. 

* **Data Cleaning:** Removed duplicates, standardized text formats (capitalization, trimming), and handled null values across customer and product tables.
* **Data Appending:** Merged regional sales data (`North Sales` and `South Sales`) into a single, unified Fact Table to streamline analysis.

*Customer Table Transformation:*
<img width="1590" height="539" alt="02_ Power Query Customer Table" src="https://github.com/user-attachments/assets/134f534a-bdba-41ee-9dc5-73537c5b5566" />


*Product Table Transformation:*
<img width="1591" height="621" alt="03_ Power Query Product Table" src="https://github.com/user-attachments/assets/4135a67f-3958-4e30-929c-828f63551162" />


*Regional Sales (North & South):*
<img width="1576" height="729" alt="04_ Power Query North Sales" src="https://github.com/user-attachments/assets/69e184a9-f0ee-43cc-9bfa-0a8a6c107224" />
<img width="1602" height="730" alt="05_ Power Query South Sales" src="https://github.com/user-attachments/assets/555b2ce1-4e33-4ed9-afbf-274f7167e299" />


*Appended Final Fact Table:*
<img width="1614" height="730" alt="06_PowerQuery Append tables" src="https://github.com/user-attachments/assets/2c799f8f-997c-4a5f-ada2-746067575f1b" />


---

## 🧩 2. Data Modeling (Star Schema)
To ensure optimal performance and accurate filtering, the data was structured using a **Star Schema** methodology.
* Established **1-to-Many** active relationships between the central Sales Fact Table and the Dimension Tables (Customers, Products, Date).
* Created a dedicated `_Measure` table to organize DAX calculations logically.

<img width="1411" height="700" alt="01_Data_Model_Star_Schema" src="https://github.com/user-attachments/assets/f804df2a-18f4-4690-ab6f-0f6a109f51f9" />


---

## 💻 3. Advanced DAX & Business Logic
Wrote dynamic DAX measures to calculate KPIs, handle potential data errors (e.g., orphaned records/blanks), and apply intelligent conditional formatting.

*Example 1: Identifying the Top Customer while filtering out blank/invalid records.*
<img width="1312" height="302" alt="10_Top Customer Name" src="https://github.com/user-attachments/assets/2a70eef6-badf-448c-b406-5093a6c0a693" />


*Example 2: Dynamic product ranking.*
<img width="1311" height="119" alt="11_ Top Product Name" src="https://github.com/user-attachments/assets/13cdd275-a7c8-4a88-ab85-79f47b075ba2" />


---

## 📈 4. Dashboard & UI/UX Design
The final interactive dashboard consists of three synchronized pages, featuring a custom navigation pane, modern UI aesthetics, and dynamic conditional formatting.

### 📄 Page 1: Sales Overview
Provides a high-level summary of total revenue, orders, and regional distribution to quickly assess overall business health.
<img width="1362" height="742" alt="07_ Over View" src="https://github.com/user-attachments/assets/b9ccefe6-e384-4d32-bc45-b96e9fe5eb86" />


### 📄 Page 2: Product Performance
Focuses on inventory success. Utilizes conditional formatting in matrices (Data Bars) and charts to automatically highlight the top 3 best-selling products.
<img width="1363" height="749" alt="08_ Product Preformance" src="https://github.com/user-attachments/assets/976ea82b-4ca6-4b50-8765-45ec068bfcdc" />


### 📄 Page 3: Customer Insights
Dives into customer segmentation and behavior over time. Features a scatter plot to identify high-value clients and a smoothed line chart to track active customer growth.
<img width="1373" height="757" alt="09_Customer" src="https://github.com/user-attachments/assets/87208077-f15b-4814-8e4a-a03e6893a1af" />


---

## 🚀 Key Skills Demonstrated
* **ETL & Data Cleaning:** Power Query M
* **Data Modeling:** Star Schema, Relational Databases
* **Data Analysis:** DAX, Time Intelligence, Logical Functions
* **Data Visualization:** UI/UX Design, Conditional Formatting, Interactive Slicers
