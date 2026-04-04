# Product-Profitability
Developed an interactive Power BI/Tableau dashboard analysing sales transactions, revenue, profit, product categories, and customer data across multiple regions.

# Project Title: Product Profitability 

This project used a business dataset containing customer, employee, product, sales and calendar data to build an interactive dashboard in Microsoft Power BI. The analysis was conducted to evaluate overall business performance and workforce effectiveness, with a focus on revenue, profit trends, product performance and sales efficiency.

The main objective was to identify key drivers of profitability, highlight high- and low-performing regions and customer segments and uncover risks such as over-reliance on specific markets and the impact of discounting on profit margins. Additionally, the project aimed to explore opportunities to improve sales performance, optimise workforce allocation and support data-driven decision-making for business growth.

[Notebook Link](https://github.com/Sodiq-Shodimu/nexygen-project/blob/main/preprocessed.ipynb)  

---

## Table of Contents

- [Overview](#overview)  
- [Dataset](#dataset)  
- [Technologies Used](#technologies-used)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Analysis & Visualizations](#analysis--visualizations)  
- [Conclusion](#conclusion)  
- [Credits](#credits)  
- [License](#license)  

---

## Overview

**Motivation:**
- I chose this dataset because it provides a comprehensive view of business operations, including sales, customers, employees and products, which makes it ideal for analysing overall business performance. The dataset allows for exploration of real-world business challenges such as revenue growth, profitability and workforce efficiency. I was particularly interested in understanding how different factors—such as customer segments, regions, and discounting—impact business success and decision-making.-

**Objective:**
- The main objective of this analysis was to evaluate business performance and identify key drivers of revenue and profit. Specifically, the project aimed to answer the following questions:
- How do revenue and profit trends change over time?
- Which products and categories contribute the most to sales and profitability?
- How effective is the sales workforce in generating revenue?
- Which regions and customer segments perform best, and where are the underperforming areas?
- What risks (e.g., heavy discounting, reliance on specific customers/regions) and opportunities exist for improving business performance?
- What question(s) are you trying to answer through this analysis?  

**Learning Outcomes:** What did you learn while working on this project?
- Through this project, I developed a stronger understanding of how to use Power BI to transform raw data into meaningful insights. I learned how to:
- Create data models by linking multiple tables (customers, sales, products, employees and calendar data).
- Build interactive dashboards to visualise trends in revenue, profit and sales performance.
- Analyse key business metrics such as profit margins and revenue per employee.
- Identify patterns, risks and opportunities within data to support strategic decision-making.
- Understand the importance of data-driven insights in improving sales strategies, workforce allocation and customer targeting.

---

## Dataset

Provide details about the dataset used:

Source of the dataset:
- The dataset used in this project is a structured business dataset containing sales, customer, product and employee data. It was used to simulate real-world business operations and support analysis within Microsoft Power BI. The dataset was provided by ITonline Learning.
  
Size of the dataset:
- The dataset is composed of multiple related tables:
- Sales Table: 1,200 rows, containing transactional sales data (largest table)
- Customer Table: 300 rows
- Products Table: 20 rows
- Employees Table: 25 rows
- Calendar Table: 730 rows (covering the full date range)
- Each table contains approximately 5–15 columns depending on the entity.

Key features/columns used:
- The analysis focused on the following key fields:
- Sales Table: Sale ID,Date, Product ID, Customer ID, Employee ID, Quantity, Unit Price, Discount, Cost Price, Revenue, Profit and High Discount Flag. 
- Customer Table: Customer ID, Region (e.g., East, North), Customer Type, Signup Date and Total Revenue 
- Products Table: ProductID, Product Name, Category (Furniture, Office Supplies, Electronics) and Cost Price
- Employees Table: Employee Name, Role and Assigned Region
- Calendar Table: Date, Year, Quarter, Month Number, Month Name and Year-Month
  
- These features were essential for analysing revenue trends, profitability, product performanc and workforce effectiveness.

Preprocessing or cleaning Steps:
- Before performing the analysis in Power BI, the dataset was prepared to ensure accuracy and consistency:
  
Data Cleaning:
- Removed duplicate records in Sales, Customers and Employees tables.
- Handled missing or null values to avoid errors in calculations (e.g., missing revenue or profit entries).
- Standardised column names and data types, especially dates in the Calendar table.

Data Transformation:
- Created calculated columns and measures:
- Profit Margin = (Profit / Revenue) × 100
- Revenue per Employee = Revenue ÷ Number of Employees
- Categorised products into groups (Furniture, Office Supplies, Electronics) for easier analysis.
  
Data Modeling:
- Established relationships between tables:
- Sales → Customers, Products, Employees, Calendar
- Ensured proper cardinality (one-to-many) and cross-filtering to allow accurate drill-through analysis.
  
Filtering and Validation:
- Checked for extreme discount values that could skew profit calculations.
- Validated regional and customer segment data to ensure correct aggregation of revenue and profit.

Time Intelligence Preparation:
- Used the Calendar table to create time-based hierarchies (Year, Month, Quarter) for revenue and profit trend analysis.
- Enabled seasonal trend analysis and comparison across years.

Dashboard-Specific Preparation:
- Added measures to support Executive Overview and Customer Drill-Through views.
- Ensured workforce allocation data was aligned with regions and sales data for performance evaluation.

---

<h2>Technologies Used</h2>

<ul>
  <li><strong>Languages & Libraries:</strong> Python, Pandas, NumPy, SQL, Matplotlib, Seaborn</li>
  <li><strong>Tools:</strong> Jupyter Notebook, VS Code, Git, GitHub</li>
  <li><strong>Data Visualization:</strong> Power BI / Tableau (if applicable)</li>
</ul>

<p>
  <img src="https://img.shields.io/badge/Excel-3776AB?style=for-the-badge&logo=Excel&logoColor=white" alt="Excel">
  <img src="https://img.shields.io/badge/Power_BI-150458?style=for-the-badge&logo=Power_BI&logoColor=white" alt="Power BI">
  <img src="https://img.shields.io/badge/DAX-013243?style=for-the-badge&logo=DAX&logoColor=white" alt="DAX">
  <img src="https://img.shields.io/badge/Power_Query-11557C?style=for-the-badge&logo=Power_Query&logoColor=white" alt="Power Query">
  <img src="https://img.shields.io/badge/CSV-4C72B0?style=for-the-badge&logo=CSV&logoColor=white" alt="CSV">

</p>

---

## Usage

Instructions for using the project:

1. Open the main notebook (`analysis.ipynb`)  
2. Run each cell sequentially to reproduce the analysis  
3. Visualizations and results will be generated automatically  

Include screenshots of your visualizations if available:  

![Visualization Example](assets/images/screenshot.png)  

<img width="2020" height="1131" alt="image" src="https://github.com/user-attachments/assets/b6ef2989-65bf-46e7-8f05-c5830971efc0" />
<img width="1433" height="1105" alt="image" src="https://github.com/user-attachments/assets/d1894bc1-702d-4f2f-b7f1-b524f3c39eb5" />


---

## Analysis & Visualizations 

Summarize your findings, insights, and visualizations:

- Describe the key trends and patterns you observed  
- Show charts, graphs, and tables  ![Graph](img1.png)
- Include important observations or correlations found in the data  

---

## Conclusion 

- Summarize the outcome of your analysis  
- What are the main insights or takeaways?  
- How could this analysis inform decision-making?  
- Recommendations or next steps for further analysis  

---

## Credits

- **Collaborators:** Name – [GitHub Profile](https://github.com/USERNAME)  
- **Dataset Source:** [Link](https://link-to-dataset.com)  
- **Tutorials / References:** [Link](https://link.com)  

---

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/) – feel free to use and modify it.  

---

<p align="center"><strong>Thanks for visiting! 🚀</strong></p>
