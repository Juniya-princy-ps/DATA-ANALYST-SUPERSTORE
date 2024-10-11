# DATA-ANALYST-SUPERSTORE
Superstore Sales & Profit Dashboard

Project Overview:

This project features a Power BI dashboard designed to provide an in-depth analysis of sales and profit data for a superstore. The dashboard offers interactive visualizations, key performance indicators, and customizable filters, enabling users to explore sales trends, shipping performance, and product category insights. It serves as a powerful tool for stakeholders to monitor business performance and make data-driven decisions.

Data Sources:

Superstore Sales Data: The data for this Power BI dashboard is sourced from a comprehensive dataset containing transactional sales data for various product categories across multiple regions.

Tools:

Power BI: Used for creating and designing the interactive dashboard.

Power Query: Utilized for cleaning and transforming the data to ensure accuracy and consistency in the analysis.

SQL: Employed for data extraction and analysis to derive key metrics efficiently.

Data Cleaning/Preparation:

Combining Data: Data from multiple sources was integrated into a single dataset for comprehensive analysis.

Handling Missing Values and Outliers: Missing values and outliers were identified and addressed using appropriate data cleaning techniques to maintain data integrity.

Standardizing Data Formats: Data formats were standardized to ensure consistency across all fields in the dataset.

Creating Calculated Columns and Measures: Key metrics such as total sales and total profit were calculated to facilitate analytical insights and visualization.

Exploratory Data Analysis (EDA):

What are the overall trends in sales and profit? The dashboard provides insights into total sales of $2.3 million and a total profit of $286.4K across all transactions.

How do different segments and categories perform? Insights reveal that the Corporate segment generates the highest profit, and Office Supplies is the leading category by 
sales quantity.

What shipping methods are most utilized? Analysis shows that Standard Class is the predominant shipping method, accounting for the majority of customer orders.

Data Analysis:
SQL

SELECT

SUM(total_sales) AS total_sales,

SUM(total_profit) AS total_profit

FROM
sales_data_table;


SELECT
segment,

SUM(total_sales) AS total_sales,

SUM(total_profit) AS total_profit

FROM
sales_data_table


GROUP BY
segment
ORDER BY

total_profit DESC;


The first SQL query calculates the total sales and total profit across all transactions. The second query analyzes performance by segment, allowing for the identification of the most profitable customer segments. This data is crucial for understanding the sales dynamics and profitability across different categories and segments in the superstore.

Results:

Overall Performance: The dashboard shows total sales of $2.3 million and total profit of $286.4K, providing a snapshot of the superstore's financial health.
Segment Insights: The Corporate segment contributed the highest profit, $134.12K, while the Consumer segment also showed strong performance, with $60.3K in profit.
Category Performance: Office Supplies led in quantity sold with 23K units, highlighting customer preferences in product selection.
Shipping Method Analysis: Most customer orders were shipped via Standard Class, indicating a potential area for optimization in logistics.

Recommendations:

Enhance Product Offerings in High-Performing Categories: Given the success of Office Supplies, consider expanding product lines in this category to capture more market share.
Focus on Corporate Customers: Develop targeted marketing strategies to further engage the Corporate segment, which has shown the highest profitability.
Optimize Shipping Processes: Given the high utilization of Standard Class shipping, explore ways to improve efficiency and reduce costs associated with shipping logistics.
