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
- Top Performers: Electronic products, predominantly from the Mobiles & Tablets category, consistently show the highest gross profit.
- Underperformers: Products with the lowest gross profit are primarily found within the School & Education, Books, and Others categories.
- Margin Discrepancy (Mobiles & Tablets): Despite contributing the highest overall gross profit, the Mobiles & Tablets category exhibits one of the lowest average Gross Profit Margins (GPM). This suggests that heavy promotional activities and discounts (as indicated by its position in the top 3 categories for average discount amount) might be impacting its profitability per unit.
- High-Margin Categories: The highest average GPMs are observed in the Home & Living, Beauty & Grooming, and Computing categories, indicating strong profitability. Low-Margin Categories: Conversely, Books, Others, and School & Education categories demonstrate the lowest average GPMs.
- Consistent Profitability: Excluding the Books and Others categories, most other categories show only slight variations in their average GPM, suggesting a generally consistent and healthy gross profit margin across the majority of the product portfolio.

#### Discount and Profitability Analysis:
- Calculate the average discount given per category and per payment_method.
- Analyze the impact of discounts on Gross Profit Margin. Do higher discounts always result in lower total Gross Profit, or is there an optimal point where discounts drive sales volume that compensates?
- **Question**: Is the current discount strategy optimal in maximizing profitability, or does it require adjustment?

**Insights**:
- Discount Distribution by Category: The Entertainment category receives the highest average discount amount ($238k), while the Books category receives the lowest ($6.95k).
- Discount Distribution by Payment Method: Jazzwallet transactions receive the highest average discount amount, totaling $1.15 million. Conversely, several payment methods, including Mygateway, Marketing Expense, MCBLite, UBL Credit Card, Product Credit, Finance Settlement, Cash at Doorstep, and Internet Banking, show no applied discounts.
- Discount Effectiveness vs. Profitability: Analysis of gross profit distribution alongside average discount amounts suggests that extensive discounting does not consistently translate into higher Gross Profit Margins (GPMs) or elevate categories into the top 5 for GPM. While discounting might boost gross profit amounts, its impact on margins is questionable.
  - Case Study: Entertainment Category: Despite receiving a high average discount, the Entertainment category remains in the bottom 5 for average GPM, and its products do not appear in the top 10 for highest total gross profit. This indicates that heavy discounting in this category is not driving significant profitability.
  - Case Study: Mobiles & Tablets Category: This category, which contributes the highest total gross profit, has an average discount of $99.98k, suggesting a more moderate discounting approach compared to Entertainment.
- Targeted Discounting (Books Category): The Books category applies discounts exclusively to transactions made via PayAxis, customer credit, and Cash on Delivery (COD), indicating a highly specific and limited discount strategy for this low-margin category.
- Overall Discount Strategy Impact: The current discount methods appear to have a limited contribution to significantly boosting overall sales. This suggests a need to re-evaluate the strategy's effectiveness in driving both sales volume and profitability.

**Recommendation**:
- Optimize Discount Strategy for High-Gross-Profit Categories: Conduct a thorough analysis and evaluation of the current marketing strategy, specifically regarding promotions and discounts. The goal is to optimize the conversion of sales volume to Gross Profit Margin (GPM) for products and categories that currently generate high gross profit but may have suboptimal margins due to aggressive discounting (e.g., Mobiles & Tablets).
- Revitalize Underperforming Products/Categories: Implement a targeted strategy to boost sales for products and categories contributing the lowest gross profit (e.g., School & Education, Books, Others). This requires re-evaluating current marketing approaches, identifying root causes for low performance, and exploring new promotional tactics or product positioning.
- Enhance Profitability in High-Traffic Payment Methods: Focus on optimizing GPM conversion for transactions utilizing Jazzwallet and Jazzvoucher. Given their high traffic driven by extensive promotions, there's an opportunity to refine discount levels or introduce alternative value propositions to improve profitability without significantly deterring sales volume.
- Expand Promotional Reach to Untapped Payment Methods: Introduce strategic promotions and discounts to payment methods that currently receive no discounts (e.g., Mygateway, Marketing Expense, MCBLite, UBL Credit Card, Product Credit, Finance Settlement, Cash at Doorstep, Internet Banking). This initiative aims to attract new customers, stimulate sales, and potentially unlock additional profit streams from these underutilized channels.

### Part 2: Pricing Analysis
#### Impact of basic_price on Sales:
- Group products by basic_price ranges (e.g., low, medium, high).
- Analyze sales (sales) and quantity trends (if calculable from sales and basic_price) for each price range.
- **Question**: How do changes in basic_price (if historical price change data is available for the same SKUs) affect the quantity sold and total sales?

**Insights**:
- Price Change Data Limitation: It was observed that there is no historical basic price change data available for the same products within the dataset. Therefore, the direct impact of price adjustments on quantity sold and total sales cannot be analyzed. However, observed changes in total quantity sold annually are likely driven by broader market trends and seasonal fluctuations.
- Quantity Trends by Price Range:
  - The Medium price range consistently shows the highest total quantity sold, closely followed by the Low price range.
  - The High price range consistently exhibits the lowest total quantity sold, likely attributable to the higher cost barrier for purchasing these products.
  - The similar total quantities observed between the Medium and Low price ranges might suggest that some products within these segments offer comparable quality with only slight feature differentiations, leading to similar consumer purchasing behaviors.
- Sales Contribution by Price Range:
  - Despite lower quantities, High-price range products contribute the highest total sales revenue, approximately $63 billion, underscoring their significant revenue impact.
  - Conversely, Low-price range products contribute the lowest total sales, at $1.57 billion.
- Product-Specific Performance within Price Ranges:
  - Within the High-price range, "Infinix_Zero 4-Grey" stands out with the highest quantity sold (67 items), generating a substantial $893 million in total sales.
  - In the Medium price range, "INDROID_BALRX&-Gold" is a top performer, having sold 2,000 items and contributed $10.37 billion to total sales.
  - "RS_Coconut Bites" is the highest contributor in terms of total quantity across all ranges (300 items sold), generating $25.23 million in total sales, highlighting its strong volume performance within its respective price segment.

#### Competitor Pricing Strategy (Assumption):
- Assume you have competitor pricing data (you can create this as dummy data or an assumption).
- Compare your basic_price with competitor prices.
- **Question**: Are there opportunities to adjust the price of certain products to increase competitiveness without significantly sacrificing profitability?

**Insights**:
- For products in the high-price range, a price adjustment of under 3% is feasible without significantly sacrificing profit. This is primarily due to their already premium pricing standard and strong brand recognition (especially for well-known brands), which allows for minor adjustments without eroding perceived value or profitability.
- Products in the medium-price range present an opportunity for price adjustments of up to 6% to significantly boost competitiveness. This range offers flexibility to attract a larger customer base by aligning more closely with competitor pricing or offering a more compelling value proposition.
- Price adjustments of up to 6% can also be considered for low-price range products, primarily aimed at boosting the quantity sold. However, given the inherently thin profit margins in this segment, a careful assessment is required. If the margins are critically thin, maintaining current pricing without adjustment might be a more prudent strategy to preserve profitability.

**Recommendations**:
- Continuous Market and Competitor Price Monitoring: Implement a robust system for continuous observation and analysis of competitor and market prices for similar products. This proactive approach is crucial to maintain competitive pricing, inform dynamic price adjustments, and sustain sales performance.
- Optimize Profit Conversion in High-Volume Segments: Focus on optimizing sales and profit conversion for products within the Low and Medium price ranges. Given their high sales performance and quantity sold, strategies should aim to enhance profitability per unit without deterring volume, potentially through refined discount strategies or value-added bundling.
- Boost Sales Volume for High-Price Range Products: Conduct a comprehensive analysis and evaluation of the marketing strategy for High-price range products. The objective is to significantly increase their quantity sales, thereby maximizing overall sales revenue and profit contribution from this high-value segment.
- Strategic Advertising and Bundling Promotions: Develop and implement targeted advertising campaigns and innovative bundling promotions. This includes strategically pairing popular items with less popular or newly introduced products to enhance product visibility, drive cross-selling, and introduce new offerings to the market.
- Leverage Technology Product Dominance: Capitalize on the strong performance of high-selling technology products (e.g., smartphones) in the High and Medium price ranges. Implement more aggressive promotions and intensify advertising efforts specifically within these categories. Concurrently, maintain a focus on continuously updating product technology improvements to foster and sustain long-term customer loyalty.

### Part 3: Inventory Analysis and Forecasting
#### Product & Category Sales Trends:
- Analyze monthly and seasonal sales trends for the Top 5 best-selling products and Top 5 best-selling categories.
- **Question**: Are there clear seasonal patterns or growth/decline trends for key products/categories?

**Insights**:
- Seasonal trend of top 5 produts:
  - IDROIX_BALRX7-Gold showed no sales activity in 2021 and the first half of 2022. However, it experienced an explosive sales performance in Q3 2022 (August-September), generating approximately $5.18 billion in sales during this period. This sudden surge and high sales performance in 2022, following no sales in 2021, strongly suggests that this is a newly launched product that quickly became a high-demand, 'hot-cake' item, reflecting a significant recent trend in technology
  - Samsung Galaxy S-7 maintained high and stable sales throughout 2021, peaking at $638.9 million in September 2021. However, its performance declined sharply, resulting in no sales in 2022. This significant decrease is likely attributed to the market's shift towards newer technology and updated product features
  - Mac-Book Pro 15 Inch demonstrated strong performance from Q2 2021 through Q2 2022, reaching its peak sales of $817.8 million in April 2022. Nevertheless, sales for this product ceased entirely in the second half of 2022
  - iPhone 7 began to establish its market dominance within the iPhone series during the last quarter of 2021. It continued to exhibit stable performance, reaching its peak sales of $513 million in March 2022
  - iPhone 6S Pro demonstrated strong sales performance throughout 2021 and into early 2022, peaking at $538 million in December 2021. Its sales performance in 2022 indicates a clear customer shift towards newer iPhone series models
- Seasonal trend of top 5 categories:
  - Mobiles & Tablets category consistently held the highest sales contribution, particularly from Q2 2021 to Q3 2022, peaking significantly in August-September 2022 with sales reaching $5.6 billion. Despite a sharp decline in Q4 2022, it remained the top-performing category, still generating $460 million in November 2022. This consistent leadership is likely driven by high demand for technology and the inherently high price points of its products
  - Enterntainment category experienced its sales peak in Q2 2022, specifically reaching $2.26 billion in April 2022. Sales subsequently declined after this peak season
  - Computing category demonstrated strong sales performance from Q3 2021 through Q2 2022, achieving its peak sales of $1.39 billion in April 2022
  - Appliance category also showed a significant contribution to sales in Q2 2022, peaking at $1.17 billion in May 2022
  - Men Fashion category The Men Fashion category reached its sales peak in Q2 2022, specifically recording $372 million in May 2022
  - Notably, all categories experienced a decrease in sales during Q4 2022. This downturn can likely be attributed to shifts in customer behavior during the year-end holiday season, where spending may shift towards non-online shopping activities or other priorities
  - Except the Mobiles & Tablets category, the remaining top-performing categories (Entertainment, Computing, Appliances, and Men Fashion) demonstrated their highest sales performance during Q2 2022. This synchronized surge across multiple categories during Q2 strongly suggests that it was driven by major seasonal events, targeted promotional campaigns, or broader market trends that significantly boosted consumer spending during that period

**Recommendations**:
- Conduct comprehensive research and analysis into market trends, customer preferences, and behavior, particularly focusing on how these factors fluctuate between peak and low seasons. Utilize these insights to develop a robust strategic marketing plan aimed at sustaining high sales performance during peak periods and effectively mitigating sharp declines during low seasons
- Implement proactive sales optimization strategies specifically targeting low seasons. This includes executing timely promotions, engaging events, or offering attractive vouchers to stimulate demand and boost sales when natural momentum is lower
- Evaluate and adapt successful marketing strategies from peak seasons for application during low seasons. This approach seeks to leverage proven methodologies to drive performance even during challenging periods
- Maintain continuous vigilance on evolving market trends, technological advancements, and shifts in consumer preferences. This proactive monitoring is crucial for adapting strategies and ensuring sustained high sales performance, particularly for high-contributing categoriesMaintain high sales performance by keep observe and the market trend and lastest update of trend

#### Demand Forecasting:
- Select 3-5 of the most important products (sku_name) (e.g., best-selling or most profitable).
- Use forecasting features in Excel/Spreadsheets (e.g., Forecast Sheet or FORECAST.ETS) to predict the sales quantity for these products for the next 3-6 months.
- **Question**: Based on demand forecasts, what is the estimated stock requirement for these products in the coming months to avoid overstock or stock-out?

#### COGS (Cost of Goods Sold) Analysis and Implications:
- Analyze the trend of COGS per unit for key products (if COGS in the column is total, you need to calculate COGS per unit).
- **Question**: Is there significant variation in COGS over time or across products? How do these COGS fluctuations affect Gross Profit Margin and pricing strategies?

**Insights**:

**Recommendations**:


