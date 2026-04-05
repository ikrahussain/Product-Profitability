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

I chose this dataset because it provides a comprehensive view of business operations, including sales, customers, employees and products, which makes it ideal for analysing overall business performance. The dataset allows for exploration of real-world business challenges such as revenue growth, profitability and workforce efficiency. I was particularly interested in understanding how different factors, such as customer segments, regions and discounting impact business success and decision-making.

**Objective:**

The main objective of this analysis was to evaluate business performance and identify key drivers of revenue and profit. Specifically, the project aimed to answer the following questions:
- How do revenue and profit trends change over time?
- Which products and categories contribute the most to sales and profitability?
- How effective is the sales workforce in generating revenue?
- Which regions and customer segments perform best, and where are the underperforming areas?
- What risks (e.g., heavy discounting, reliance on specific customers/regions) and opportunities exist for improving business performance?
- What question(s) are you trying to answer through this analysis?  

**Learning Outcomes:**

Through this project, I developed a stronger understanding of how to use Power BI to transform raw data into meaningful insights. I learned how to:
- Create data models by linking multiple tables (customers, sales, products, employees and calendar data).
- Build interactive dashboards to visualise trends in revenue, profit and sales performance.
- Analyse key business metrics such as profit margins and revenue per employee.
- Identify patterns, risks and opportunities within data to support strategic decision-making.
- Understand the importance of data-driven insights in improving sales strategies, workforce allocation and customer targeting.

---

## Dataset

Provide details about the dataset used:

Source of the dataset:
- The dataset used in this project is a structured business dataset containing sales, customer, product and employee data.
- It was used to simulate real-world business operations and support analysis within Microsoft Power BI. The dataset was provided by ITonline Learning.
  
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
  
These features were essential for analysing revenue trends, profitability, product performance and workforce effectiveness.

Preprocessing or cleaning Steps:

Before performing the analysis in Power BI, the dataset was prepared to ensure accuracy and consistency:
  
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

![Visualization Example](assets/images/screenshot.png)  

<img width="2020" height="1131" alt="image" src="https://github.com/user-attachments/assets/b6ef2989-65bf-46e7-8f05-c5830971efc0" />
<img width="1433" height="1105" alt="image" src="https://github.com/user-attachments/assets/d1894bc1-702d-4f2f-b7f1-b524f3c39eb5" />


---

## Analysis & Visualizations 

1. Revenue and Profit Trends:
- Revenue shows steady growth over time with clear seasonal peaks, largely driven by corporate customers in the East and North regions.
- Profit remains mostly stable but is sensitive to high discounting, which can reduce profit margins.
- Observation: There is a positive correlation between the regions with higher corporate customer activity and overall revenue growth.

<img width="400" height="368" alt="image" src="https://github.com/user-attachments/assets/a4a05aa0-8a39-4079-8e4f-80c1482d059c" />

2. Top Products and Categories:
- Furniture generates the highest overall revenue and profit.
- Office Supplies and Accessories show steady sales growth but have lower profit margins.
- Electronics sales are increasing, though at a lower volume.
- Observation: High-volume products like Furniture drive profit, while low-volume products like Electronics present growth opportunities.
  

<img width="578" height="728" alt="image" src="https://github.com/user-attachments/assets/d1e6a90d-c7e1-40c1-914d-dfe1e58ed08d" />



3. Sales Workforce Effectiveness:
   - Sales output is relatively balanced, but Revenue per Employee can be improved by targeting high-demand regions and customer segments.
   - Example: Focusing sales in the East region with corporate customers can maximize revenue.
   - Conversely, underperforming regions and customer segments present opportunities for promotional campaigns and sales realignment.


  <img width="401" height="378" alt="image" src="https://github.com/user-attachments/assets/03f06589-8adc-4efb-9207-41e512722223" />



4. Risks and Opportunities

Risks:
- Heavy discounting reduces overall profit margins.
- Dependence on corporate customers and the Eastern region makes the business vulnerable to changes in these markets.

Opportunities:
- Increase sales in underperforming regions by adjusting inventory, marketing and promotions.
- Enhance customer retention through personalized offers based on past purchases.
- Optimize workforce allocation by assigning sales staff to high-value regions and customer segments.


<img width="665" height="369" alt="image" src="https://github.com/user-attachments/assets/732c0ee7-60b7-496e-9064-6bef53c48dba" />



---

## Conclusion 

Summary of the Analysis:

This project analysed business performance and workforce effectiveness using an interactive Power BI dashboard. The analysis revealed steady revenue growth with seasonal fluctuations, stable profit margins affected by discounting and clear differences in performance across product categories, regions and customer segments. It also highlighted how workforce allocation and customer targeting influence overall sales outcomes.

Main Insights / Takeaways:

Revenue Growth Drivers: 
- Corporate customers in the East and North regions are the primary contributors to revenue growth.

Profitability Risks: 
- High discount levels negatively impact profit margins, despite strong sales performance.

Product Performance: 
- Furniture is the most profitable category, while Office Supplies have lower margins and Electronics show growth potential.

Workforce Efficiency: 
- Sales performance is balanced, but revenue per employee can be improved through better regional and customer alignment.

Business Dependency Risk: 
- The company is heavily reliant on specific regions and customer segments, increasing vulnerability.

How This Analysis Informs Decision-Making:

- Helps management identify high-performing regions and customer segments to prioritise investment.
- Supports pricing and discount strategies to protect profit margins.
- Enables data-driven workforce planning, ensuring employees are assigned to areas with the highest potential return.
- Highlights underperforming areas, allowing targeted marketing and sales strategies to improve performance.
- Provides insight into risk exposure, encouraging diversification of customers and regions.


Recommendations / Next Steps:

- Reduce excessive discounting to improve overall profitability.
- Diversify the customer base and regions to reduce reliance on corporate clients in specific areas.
- Target underperforming regions with marketing campaigns and improved product availability.
- Increase customer retention through personalised promotions based on purchase history.
- Optimise workforce allocation by assigning sales staff to high-demand regions and customer segments.

Further Analysis:
- Conduct deeper customer segmentation (e.g., behaviour or purchase frequency).
- Analyse long-term trends to improve forecasting.
- Explore product-level profitability to refine pricing and inventory strategies.

---

## Credits


- **Collaborators:** Name – [GitHub Profile](https://github.com/USERNAME)  
- **Dataset Source:** [Link]([https://link-to-dataset.com](https://www.itonlinelearning.com/?utm_feeditemid=&utm_device=c&utm_term=itonlinelearning&utm_source=google&utm_medium=ppc&utm_campaign=ITonlinelearning+UK+2021&hsa_cam=6491997354&hsa_grp=79332809913&hsa_mt=e&hsa_src=g&hsa_ad=391784972313&hsa_acc=1636904472&hsa_net=adwords&hsa_kw=itonlinelearning&hsa_tgt=kwd-365009355317&hsa_ver=3&gad_source=1&gad_campaignid=6491997354&gbraid=0AAAAAD0JJNVDJdFiQunigWAsfYUFko_qM&gclid=EAIaIQobChMIvv3Hms7WkwMVnZpQBh3SSBX-EAAYASAAEgJofPD_BwE))  

---

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/) 

---

<p align="center"><strong>Thanks for visiting! 🚀</strong></p>
