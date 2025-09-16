

# Retail Sales & Finance Dashboard

### An End-to-End Data Analytics Project

This project showcases a complete data analysis pipeline, from raw data cleaning and transformation to building an interactive business intelligence dashboard. Using a retail sales dataset, the project provides key insights into financial performance, customer trends, and sales forecasting.

-----

## 🚀 Key Features

  * **Data Cleaning & Preprocessing (Python):** Wrote a Python script using `Pandas` to clean and prepare raw sales data, handling missing values, standardizing formats, and correcting data types.
  * **SQL-Based Business Analytics:** Developed and executed complex SQL queries to calculate core business KPIs, including total revenue, profit margin, and customer acquisition trends.
  * **Dynamic Reporting Dashboard (Excel):** Built a multi-page, interactive dashboard in Excel using Pivot Tables and Charts. The dashboard features dynamic slicers to filter data by category, region, and time.
  * **Sales Forecasting:** Implemented a simple linear regression model in Python's `scikit-learn` to forecast future sales trends, demonstrating skills in predictive analytics.
  * **Variance Analysis:** Compared actual sales against a hypothetical budget to calculate performance variance and identify key business gaps.

-----

## 🛠️ Technologies Used

  * **Python:** `Pandas`, `Matplotlib`, `scikit-learn`
  * **SQL:** SQLite
  * **Excel:** Pivot Tables, Charts, Slicers
  * **Jupyter Notebook** (for initial analysis and a project walkthrough)

-----

## 📊 Project Walkthrough & Insights

### **1. Data Cleaning**

The raw dataset contained inconsistent formats and missing values. The Python script was used to clean the data and save it as a structured CSV file, ready for analysis.

 
<img width="1721" height="554" alt="image" src="https://github.com/user-attachments/assets/311fe2ba-9ecf-4760-9798-a5bf18da68ca" />
<img width="1696" height="672" alt="image" src="https://github.com/user-attachments/assets/bb2260d4-4c42-4162-a758-2240bb2e4ceb" />
<img width="1703" height="542" alt="image" src="https://github.com/user-attachments/assets/2a64917d-6022-40e6-9513-adef33183710" />

### **2. Core Business Analysis (SQL)**

SQL queries were used to answer critical business questions.

**Query 1: Overall Financial Performance**
This query calculates total revenue, profit, and the overall profit margin for the business.

```sql
SELECT
    SUM(Sales) AS Total_Revenue,
    SUM(Profit) AS Total_Profit,
    (SUM(Profit) / SUM(Sales)) * 100 AS Profit_Margin_Percentage
FROM
    Superstore_Sales_Cleaned;
```

**Query 2: Sales & Profit by Category and Region**
This query identifies the top-performing categories and regions, which helps a business prioritize its resources.

```sql
SELECT
    Category,
    Region,
    SUM(Sales) AS Total_Sales,
    SUM(Profit) AS Total_Profit
FROM
    Superstore_Sales_Cleaned
GROUP BY
    Category,
    Region
ORDER BY
    Total_Sales DESC;
```

### **3. Interactive Dashboard**

The cleaned data was imported into Excel to create a dynamic dashboard. Key visualizations include:

  * Sales and Profit by Product Category
  * Sales over Time (to identify trends)
  * Profit by Geographic Region

 
<img width="1920" height="1080" alt="Screenshot (248)" src="https://github.com/user-attachments/assets/35065270-65ee-4ddd-8cb0-d1641bab37ff" />
<img width="1920" height="1080" alt="Screenshot (249)" src="https://github.com/user-attachments/assets/cfe138ef-e30c-4599-887f-923affde5e4e" />
<img width="1920" height="1080" alt="Screenshot (247)" src="https://github.com/user-attachments/assets/f56a7ddd-74c3-439d-9006-d5082143206c" />




### **4. Sales Forecasting**

A linear regression model was built in Python to forecast sales for the upcoming months. This serves as a basis for future budget planning and demand forecasting.

 
<img width="1032" height="545" alt="download" src="https://github.com/user-attachments/assets/e44dd30a-c511-4dcd-a600-ca84b1c603e4" />

-----

## 📈 **Project Impact**

This project demonstrates the ability to translate raw data into actionable business insights. The dashboard and analysis can help stakeholders:

  * Quickly monitor business performance against goals.
  * Identify high-performing and underperforming areas.
  * Make data-driven decisions on budget and strategy.

-----

**Connect with me:**  https://github.com/mayankahuja-pro/
