# data_presentation_visuals
This project explores the Sample Superstore dataset using multiple analytical tools — Excel, Power BI, Tableau, SQL, and Python (Google Colab).
The goal is to uncover key business insights such as:

Which categories and regions drive the most sales and profit

Yearly and monthly trends

Top products and customer segments



Tools Used

Tool	Purpose
Excel	Data cleaning, pivot tables, charts, KPI summaries
Python (Google Colab)	Data preprocessing, exploratory data analysis (EDA), and visualizations
SQL	Querying and aggregating key business metrics
Power BI	Interactive dashboard with filters (slicers) for dynamic analysis
Tableau Public	Web-based dashboard for sharing visual insights


Key Insights

Technology and Office Supplies categories generate the highest sales.

Western and Eastern regions show stronger profitability.

Discounts beyond 20% significantly reduce overall profit margins.

California and New York lead in both sales volume and profit.

Consumer segment contributes the largest revenue share.



Dashboards


Power BI Dashboard

Includes:

Sales and Profit by Region and Category

Monthly and Yearly Sales Trend

Top 10 Products by Profit

Interactive filters for Region, Category, Segment, and Year

Download Power BI file:
Link would be provided later



Tableau Dashboard

Includes:

Sales & Profit Heat Map

Sales by Category and Region

Profit Ratio per Product Sub-Category

View on Tableau Public: tableau/superstore_tableau.twb




Python Analysis (Google Colab)

Performed data cleaning and feature engineering:

Converted dates to datetime format

Added new columns: Order Year, Order Month, and Profit Margin

Visualized sales and profit trends using Matplotlib and Seaborn

Notebook: collab/superstore (1).ipynb

For more information: 
https://colab.research.google.com/drive/1C_cPAPUjhZh1Gh803172hrwMKB0zrsBA#scrollTo=7h8gW0VCkX20




Excel Analysis

Created pivot tables and visual charts:

Sales by Category & Region

Profit by Product

Trend analysis by Month and Year

Discount vs. Profit correlation

File: excel/Superstore_final_excel.xlsx




SQL Queries

Sample queries used for aggregation and validation:

-- Total Sales and Profit by Category
SELECT Category, SUM(Sales) AS Total_Sales, SUM(Profit) AS Total_Profit
FROM Superstore
GROUP BY Category
ORDER BY Total_Sales DESC;

-- Yearly Sales Trend
SELECT YEAR(Order_Date) AS Year, SUM(Sales) AS Sales
FROM Superstore
GROUP BY YEAR(Order_Date)
ORDER BY Year;




How to Reproduce (Open it on your workspace)

Clone the repository:

git clone [https://github.com/your-username/superstore-analytics.git](https://github.com/tanushikxd/data_presentation_visuals)


Open the Jupyter/Colab notebook and run the analysis.

Load Superstore_corrected.csv into Power BI, Tableau, or Excel to explore the dashboards.





Conclusion

This project demonstrates how data from a retail business can be analyzed across different tools to support decision-making.
Each tool brings unique strengths:

Excel for quick exploration,

Python for automation,

Power BI/Tableau for interactive visualization,

SQL for data integrity checks.
