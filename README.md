# DUMMY-PROJECT-INVENTORY-PRICING-&-PROFITABILITY-DATA-ANALYSIS
## OVERVIEW
This project showcases a comprehensive data analysis workflow focused on inventory, pricing, and profitability, designed to provide actionable insights for business decision-making. Utilizing a combination of Excel and Power BI, the project demonstrates proficiency in data transformation, visualization, and advanced analytical techniques.

### Key Features:
- Data Preparation & Transformation: Leveraged Power Query in Excel for robust data cleaning, reshaping, and transformation of raw sales data into an analytical-friendly structure.
- Profitability Analysis: Conducted in-depth analysis of gross profit margins across various product categories, effectively identifying both high-performing and underperforming products/categories to highlight areas for strategic focus.
- Sales Performance Tracking: Developed visualizations for top N and bottom N best-selling products, providing clear insights into overall product performance and market trends.
- Time-Series Analysis & Forecasting: Implemented advanced forecasting techniques for high-performance products and key categories, generating 6-month sales predictions to proactively inform inventory management and strategic planning.
- Interactive Dashboard Development: Designed and built an interactive Power BI dashboard to visualize indicators related to sales, gross profit, and future forecasts for intuitive data exploration.
- Dynamic Filtering & Slicers: Incorporated interactive slicers (e.g., Price Range, Order Date) to empower users with dynamic data exploration capabilities, enabling focused analysis and personalized insights.
  
This project highlights skills in data modeling, business intelligence, and delivering data-driven insights crucial for optimizing inventory management, refining pricing strategies, and enhancing overall profitability.

## TOOL USED
This project effectively leverages a suite of Microsoft tools for comprehensive data handling, analysis, and visualization:
- **Power Query (within Excel/Power BI)**: Utilized extensively for robust data cleaning, reshaping, and transformation processes. It ensured the raw data was validated and prepared into a clear, structured, and analysis-ready format.
- **Microsoft Excel**: Employed for in-depth data analysis and extraction, particularly through the use of PivotTables to derive crucial insights into sales performance and profit distribution across various products and categories. Excel's built-in forecasting features were also instrumental in calculating and predicting sales performance for top-selling products and categories, aiding in strategic marketing planning and inventory management.
- **Microsoft Power BI**: The primary tool for developing an interactive and intuitive dashboard. It facilitated the visualization of complex analyses in a clear and easily digestible format. Power BI's capabilities were leveraged to connect diverse data sources and to build enhanced data models (e.g., custom date tables, DAX measures) for deeper data exploration and insightful reporting.

## KEY FINDINGS, INSIGHTS, AND RECOMMENDATIONS
### Part 1: Profitability Analysis
##### Profitability Calculation:
- Calculate Gross Profit for each transaction (Sales - COGS).
- Calculate Gross Profit Margin (as a percentage) for each transaction.
- Identify the Top 10 and Bottom 10 products (sku_name) based on total Gross Profit over the available data period.
- Identify the Top 5 and Bottom 5 categories (category) based on Gross Profit Margin.
- **Question**: How is profitability distributed across products and categories? Are there products or categories with high sales but low margins, or vice versa?

**Insights**:

#### Discount and Profitability Analysis:
- Calculate the average discount given per category and per payment_method.
- Analyze the impact of discounts on Gross Profit Margin. Do higher discounts always result in lower total Gross Profit, or is there an optimal point where discounts drive sales volume that compensates?
- **Question**: Is the current discount strategy optimal in maximizing profitability, or does it require adjustment?

**Insights**:

**Recommendation**:

### Part 2: Pricing Analysis
#### Impact of basic_price on Sales:
- Group products by basic_price ranges (e.g., low, medium, high).
- Analyze sales (sales) and quantity trends (if calculable from sales and basic_price) for each price range.
- **Question**: How do changes in basic_price (if historical price change data is available for the same SKUs) affect the quantity sold and total sales?

#### Competitor Pricing Strategy (Assumption):
- Assume you have competitor pricing data (you can create this as dummy data or an assumption).
- Compare your basic_price with competitor prices.
- **Question**: Are there opportunities to adjust the price of certain products to increase competitiveness without significantly sacrificing profitability?

**Insights**:

**Recommendations**:

### Part 3: Inventory Analysis and Forecasting
#### Product & Category Sales Trends:
- Analyze monthly and seasonal sales trends for the Top 5 best-selling products and Top 5 best-selling categories.
- **Question**: Are there clear seasonal patterns or growth/decline trends for key products/categories?

#### Demand Forecasting:
- Select 3-5 of the most important products (sku_name) (e.g., best-selling or most profitable).
- Use forecasting features in Excel/Spreadsheets (e.g., Forecast Sheet or FORECAST.ETS) to predict the sales quantity for these products for the next 3-6 months.
- **Question**: Based on demand forecasts, what is the estimated stock requirement for these products in the coming months to avoid overstock or stock-out?

#### COGS (Cost of Goods Sold) Analysis and Implications:
- Analyze the trend of COGS per unit for key products (if COGS in the column is total, you need to calculate COGS per unit).
- **Question**: Is there significant variation in COGS over time or across products? How do these COGS fluctuations affect Gross Profit Margin and pricing strategies?

**Insoghts**:

**Recommendations**:


