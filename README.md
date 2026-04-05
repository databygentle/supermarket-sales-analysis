 Supermarket Sales Analysis: Insights for Retail Decision-Making

I performed data cleaning, exploratory data analysis (EDA), and trend visualization on the supermarket sales dataset (covering Naypyitaw, Yangon, and Mandalay) to identify high-value spending patterns and key sales drivers to optimize operational decision-making.

 Dataset

Source: The dataset is sourced from the Supermarket Sales Analysis repository on GitHub, originally providing a historical record of sales from a supermarket company recorded over three months.

Dimensions:
- Rows: 1,000
- Columns: 16 (after removing the `gross margin percentage` column during the data cleaning phase)

Description: This dataset captures transaction-level details from three different supermarket branches located in Naypyitaw, Yangon, and Mandalay. It is designed for retail analytics, specifically to study sales trends, customer behavior, and product performance over the first quarter of the year (January to March).

Key Information Contained:
- Transaction Details: Unique `Invoice ID`, the specific `Branch` (A, B, or C), and the `City` where the sale occurred
- Customer Demographics: Information on `Customer type` (Member or Normal) and `Gender`
- Product Categories: A variety of `Product lines` ranging from "Health and beauty" to "Electronic accessories"
- Financial Data: Critical numerical values including `Unit price`, `Quantity` purchased, `Tax 5%`, and the `Total` transaction amount
- Operational Data: Cost of goods sold (`cogs`), the `Payment` method used (Ewallet, Cash, or Credit card), and the customer `Rating` for the shopping experience
- Temporal Data: The specific `Date` and `Time` of each purchase, allowing for the analysis of peak shopping periods and monthly trends

 Objectives

The main goal of this project is to analyze supermarket sales data and extract actionable insights to support business decision-making. This project set out to answer the following specific questions:

- Sales Over Time: What are the sales trends in different cities from January to March?
- Top Revenue Product: Which product line generates the most revenue?
- Customer Favorites: Which product line has the highest customer ratings?
- Membership Value: Do members spend more money than normal customers?
- High-Value Customers: What is the spending behavior of high-value customers?
- Best Sales Period: Which time of the month generates the most sales?
- Top Performing City: Which city has the highest total sales?

 Tools & Libraries

- Python: The main programming language used for writing the analysis scripts
- Jupyter Notebook: The interactive environment where the code was written and executed
- Pandas: Used for loading the dataset, cleaning the data, and calculating aggregations
- Matplotlib: Used to control figure size, axis formatting, and plot layout
- Seaborn: Used to create bar charts, line plots, and histograms with a clean, modern look

 Process Summary

- Loaded the dataset and imported the necessary libraries (Pandas, Matplotlib, and Seaborn) to start the analysis
- Conducted data profiling to get an overview of the 1,000 rows, inspect data types, and check for any missing values
- Identified and resolved data quality issues including dropping the unnecessary `gross margin percentage` column and ensuring the Date and Time columns were in the correct format for analysis
- Engineered a new column to extract the Month from the original data, allowing for a deeper look at time-based sales trends
- Built visualizations to answer key business questions, such as identifying the highest-selling cities, peak sales months, and the spending behavior of high-value customers

 Key Findings

- Sales Trends Across Cities: Sales show clear weekly fluctuations in all cities, with Naypyitaw consistently generating the highest revenue, while Yangon and Mandalay display more similar but lower patterns
- Product Line Revenue: Home and Lifestyle generates the highest revenue among all product lines, followed closely by Sports and Travel, while Fashion Accessories contributes the least
- Customer Ratings: Food and Beverages receives the highest average customer rating, indicating strong customer satisfaction in this category
- Member vs Normal Customers: Members spend slightly more than normal customers, but the difference in total revenue between the two groups is very small
- High-Value Customer Spending: The number of high-value customers decreases as the transaction value increases
- Sales by Month: January had the most sales, followed by March, and February had the least. While the differences are visible, the margin between them is not significant
- Sales by City: Naypyitaw has the highest sales volume, followed by Mandalay, and Yangon has the least, with no significant margin differences between the three cities

 Recommendations

- Sales Trends Across Cities: The supermarket should diversify its product offerings across cities to reduce dependency on any single category and buffer against sales volatility
- Product Line Revenue: All product lines should be treated with equal importance, and the availability of goods across all categories should be carefully maintained
- Customer Ratings: Since the highest-revenue category has the lowest rating, management should investigate why customers rated it poorly. They should also prioritise the availability of highly rated product lines to drive both satisfaction and revenue
- Member vs Normal Customers: Both customer types should be prioritised due to the insignificant margin between them, while also implementing strategies to convert normal customers into members
- High-Value Customer Spending: The supermarket should work to increase high-value customers by improving the perceived value of its products, offering discounts for larger purchases, and creating positive experiences to retain them
- Sales by Month: Stock availability should be maximised in January to meet high demand, maintained adequately in March, and further investigation should be conducted into February's lower performance
- Sales by City: The supermarket should investigate potential market expansion opportunities in Yangon, where sales are lowest, to strengthen its competitive position in that city

## How to Run

1. Clone this repository or download the `.ipynb` file
2. Install the required libraries: `pip install pandas numpy matplotlib seaborn`
3. Download the dataset from GitHub: https://github.com/sushantag9/Supermarket-Sales-Data-Analysis/blob/master/supermarket_sales%20-%20Sheet1.csv
4. Place the dataset in the same folder as the notebook
5. Open Jupyter Notebook and run the cells in order
