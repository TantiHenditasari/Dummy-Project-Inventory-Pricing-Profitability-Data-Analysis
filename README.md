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

<img width="473" height="225" alt="image" src="https://github.com/user-attachments/assets/75a69b2e-a123-4d5f-b7da-d9712dfaf71a" />
<img width="474" height="225" alt="image" src="https://github.com/user-attachments/assets/110fd0e5-8cc6-4312-941e-10114e967b4c" />
<img width="476" height="221" alt="image" src="https://github.com/user-attachments/assets/a48a0abc-3f46-4465-b9d2-7324f12cb8dd" />

**Insights**:
- Top Performers: Electronic products, predominantly from the Mobiles & Tablets category (such as products from iPhone, Samsung, and IDROIX) consistently show the highest gross profit, generating total gross profit ranging from $300 to $500 M .
- Underperformers: Products with the lowest gross profit are primarily found within the School & Education, Books, and Others categories. Notably, the 4U_Service product exhibit the lowest total gross profit at -$23.66k. This negative value is likely a result of the heavy discounts applied to this product, which our analysis shows can significantly decrease overall gross profit.
- High-Margin Categories: The highest average GPMs are observed in the Home & Living, Beauty & Grooming, Mobiles & Tablet, and Men Fashion categories at 92.58% - 92.71%, indicating strong profitability. Low-Margin Categories: Conversely, Books, Others, and School & Education categories demonstrate the lowest average GPMs at 84.86% - 92.22%.
- Excluding the Books and Others categories, most other categories show only slight variations in their average GPM, suggesting a generally consistent and healthy gross profit margin across the majority of the product portfolio.

#### Discount and Profitability Analysis:
- Calculate the average discount given per category and per payment_method.
- Analyze the impact of discounts on Gross Profit Margin. Do higher discounts always result in lower total Gross Profit, or is there an optimal point where discounts drive sales volume that compensates?
- **Question**: Is the current discount strategy optimal in maximizing profitability, or does it require adjustment?

<img width="1013" height="571" alt="image" src="https://github.com/user-attachments/assets/9423af4c-7f64-4190-b84b-d49799d2ad7a" />

**Insights**:
- The Appliances category receives the highest average discount amount ($171.49k), while the Books category receives the lowest ($4.77k).
- Jazzwallet transactions receive the highest average discount amount, totaling $1.27 million. Conversely, several payment methods, including Mygateway, Marketing Expense, MCBLite, UBL Credit Card, Product Credit, Finance Settlement, Cash at Doorstep, EasyPay Voucher and Internet Banking, show no applied discounts.
- Analysis of gross profit distribution alongside average discount amounts suggests that extensive discounting does not consistently translate into higher Gross Profit Margins (GPMs) or elevate categories into the top 5 for GPM. While discounting might boost gross profit amounts, its impact on margins is questionable.
  - Case Study: Appliances and Others Category: Despite receiving the highest average discount, these categories remains in the bottom 5 for average GPM contributing 92.37% and 91.45%, and their products do not appear in the top 10 for the best-selling by total gross profit. This indicates that heavy discounting in these categories is ineffective, failing to drive significant profitability despite high discount amounts.
  - Case Study: Mobiles & Tablets Category: This category, which contributes the highest total gross profit, has an average discount of $52.94k and contributing GPM in 92.58% in the third highest contributor, suggesting a more moderate discounting approach compared to Appliances.
- The Books category applies discounts exclusively to transactions made via PayAxis, customer credit, and Cash on Delivery (COD), indicating a highly specific and limited discount strategy for this low-margin category.
- The current discount methods appear to have a limited contribution to significantly boosting overall sales. This suggests a need to re-evaluate the strategy's effectiveness in driving both sales volume and profitability.

**Recommendation**:
- Conduct a thorough analysis and evaluation of the current marketing strategy, specifically regarding promotions and discounts to optimize the conversion of sales volume to Gross Profit Margin (GPM) for products and categories that currently generate high gross profit but may have suboptimal margins due to high discounting (e.g., Mobiles & Tablets).
- Re-evaluate and re-calculate for the categories with the highest discount campaign that still could not contribute in converting high GPM (e.g., Appliances and Others) to reduce the lost of Gross Profit and GPM.
- Implement a targeted strategy to boost sales for products and categories contributing the lowest gross profit (e.g., School & Education, Books, Others). This requires re-evaluating current marketing approaches, identifying root causes for low performance, and exploring new promotional tactics or product positioning.
- Enhance Profitability in High-Traffic Payment Methods: Focus on optimizing GPM conversion for transactions utilizing Jazzwallet and Jazzvoucher. Given their high traffic driven by extensive promotions, there's an opportunity to refine discount levels or introduce alternative value propositions to improve profitability without significantly deterring sales volume.
- Expand Promotional Reach to Untapped Payment Methods: Introduce strategic promotions and discounts to payment methods that currently receive no discounts (e.g., Mygateway, Marketing Expense, MCBLite, UBL Credit Card, Product Credit, Finance Settlement, Cash at Doorstep, Internet Banking). This initiative aims to attract new customers, stimulate sales, and potentially unlock additional profit streams from these underutilized channels.

### Part 2: Pricing Analysis
#### Impact of basic_price on Sales:
- Group products by basic_price ranges (e.g., low, medium, high).
- Analyze sales (sales) and quantity trends (if calculable from sales and basic_price) for each price range.
- **Question**: How do changes in basic_price (if historical price change data is available for the same SKUs) affect the quantity sold and total sales?

<img width="945" height="221" alt="image" src="https://github.com/user-attachments/assets/9ad0629a-1068-418b-9941-54590935cbc7" />
<img width="946" height="223" alt="image" src="https://github.com/user-attachments/assets/9090f829-ad60-4598-9590-c6cc36f16a35" />

**Insights**:
- It was observed that there is no historical basic price change data available for the same products within the dataset. Therefore, the direct impact of price adjustments on quantity sold and total sales cannot be analyzed. However, observed changes in total quantity sold annually are likely driven by broader market trends and seasonal fluctuations.
- The Low price range consistently shows the highest total quantity sold at 3.8k items, closely followed by the Medium price range at 3.5k items.
- The High price range consistently exhibits the lowest total quantity sold at 763 items, likely attributable to the higher cost barrier for purchasing these products.
- The similar total quantities observed between the Medium and Low price ranges might suggest that some products within these segments offer comparable quality with only slight feature differentiations, leading to similar consumer purchasing behaviors.
- Despite lower quantities, High-price range products contribute the highest total sales revenue, approximately $23.44 billion, underscoring their significant revenue impact.
- Conversely, Low-price range products contribute the lowest total sales, at $1.05 billion.
- Within the High-price range, "Samsung_40K5000" stands out with the highest quantity sold (21 items), generating a substantial $602 million in total sales in 2022.
- In the Medium price range, "INDROID_BALRX&-Gold" is a top performer, having sold 1k items and contributed $5.18 billion to total sales in 2022. This product contributes highest sales across all of price range during this 2 years. This exceptional performance suggests that INDROID_BALRX&-Gold was a top-selling or trending product in 2022
- "RB_Dettol Germ Busitng Kit-bf" is the highest contributor in terms of total quantity across low-priced items (240 items sold), generating $25.23 million in total sales in 2021 - 2022.

#### Competitor Pricing Strategy (Assumption):
- Assume you have competitor pricing data (you can create this as dummy data or an assumption).
- Compare your basic_price with competitor prices.
- **Question**: Are there opportunities to adjust the price of certain products to increase competitiveness without significantly sacrificing profitability?

**Insights**:
- For products in the high-price range, a price adjustment of under 3% is feasible without significantly sacrificing profit. This is primarily due to their already premium pricing standard and strong brand recognition (especially for well-known brands), which allows for minor adjustments without eroding perceived value or profitability.
- Products in the medium-price range present an opportunity for price adjustments of up to 6% to significantly boost competitiveness. This range offers flexibility to attract a larger customer base by aligning more closely with competitor pricing or offering a more compelling value proposition.
- Price adjustments of up to 6% can also be considered for low-price range products, primarily aimed at boosting the quantity sold. However, given the inherently thin profit margins in this segment, a careful assessment is required. If the margins are critically thin, maintaining current pricing without adjustment might be a more prudent strategy to preserve profitability.

**Recommendations**:
- Implement a robust system for continuous observation and analysis of competitor and market prices for similar products. This proactive approach is crucial to maintain competitive pricing, inform dynamic price adjustments, and sustain sales performance.
- Focus on optimizing sales and profit conversion for products within the Low and Medium price ranges. Given their high sales performance and quantity sold, strategies should aim to enhance profitability per unit without deterring volume, potentially through refined discount strategies or value-added bundling.
- Conduct a comprehensive analysis and evaluation of the marketing strategy for High-price range products to significantly increase their quantity sales, thereby maximizing overall sales revenue and profit contribution from this high-value segment.
- Develop and implement targeted advertising campaigns and innovative bundling promotions. This includes strategically pairing popular items with less popular or newly introduced products to enhance product visibility, drive cross-selling, and introduce new offerings to the market.
- Capitalize on the strong performance of high-selling technology products (e.g., smartphones and other electronic products) in the High and Medium price ranges. Implement more aggressive promotions and intensify advertising efforts specifically within these categories. Concurrently, maintain a focus on continuously updating product technology improvements to foster and sustain long-term customer loyalty.

### Part 3: Inventory Analysis and Forecasting
#### Product & Category Sales Trends:
- Analyze monthly and seasonal sales trends for the Top 5 best-selling products and Top 5 best-selling categories.
- **Question**: Are there clear seasonal patterns or growth/decline trends for key products/categories?

<img width="945" height="220" alt="image" src="https://github.com/user-attachments/assets/e868779d-31f7-46ac-afe9-06a6d01ea18e" />
<img width="863" height="631" alt="image" src="https://github.com/user-attachments/assets/03b257bf-364d-4ef2-a60d-90d5acacf38d" />

**Insights**:
- Seasonal trend of top 5 produts:
  - IDROIX_BALRX7-Gold showed no sales activity in 2021 and the first half of 2022. However, it experienced an explosive sales performance in Q3 2022 (September), generating approximately $5.18 billion in sales during this period. This sudden surge and high sales performance in 2022, following no sales in 2021, strongly suggests that this is a newly launched product that quickly became a high-demand, 'hot-cake' item, reflecting a significant recent trend in technology
  - Samsung_40K5000 also demonstrate no sales throughout 2021. However, its performance inclined sharply in April 2022 (Q2) generating $602 million that also strongly suggest that this product is new launced and being a trending product especially do to the bulking purchase.
  - iPhone 6S Plus 16GB Silver demonstrated strong sales performance throughout 2021 and into early 2022, peaking at $301 million in December 2021 (Q4). Its sales performance in 2022 indicates a clear customer shift towards newer iPhone series models due to this produt exhibites no sales after January 2022
  - iPhone SE-16GB contribute its highest sales in August 2021 (Q3), generating $502 million. Likely iPhone 6S Plus, this product drops its sales significantly after its peak and show no sales after it that might be due to the shifting trend of iPhone series.
  - Samsung Galaxy S-7 32GB LTE demonstrate the stabile sales during June - October 2021 (Q2 - Q4) and peaked in August 2021 by $149 million. However, this product had no sales anymore in 2022.
- Seasonal trend of top 5 categories:
  - Mobiles & Tablets category consistently held the highest sales contribution, particularly from Q2 2021 to Q3 2022, peaking significantly in September 2022 with sales reaching $5.2 billion. Despite a sharp decline in Q4 2022, it remained the top-performing category, still generating $157 million in December 2022. This consistent leadership is likely driven by high demand for technology and the inherently high price points of its products
  - Appliance category also showed a significant contribution to sales in Q1 - Q2 2022, peaking at $498 million in April 2022
  - Enterntainment category experienced its sales peak in Q2 2022, specifically reaching $947 million in April 2022. Sales subsequently declined after this peak season
  - Computing category demonstrated strong sales performance Q4 2021, achieving its peak sales of $522 million in December 2021
  - Men Fashion category The Men Fashion category reached its sales peak in Q1 - Q2 2022, specifically recording $264 million in May 2022
  - Notably, all categories experienced a decrease in sales during Q4 2022. This downturn can likely be attributed to shifts in customer behavior during the year-end holiday season, where spending may shift towards non-online shopping activities or other priorities
  - Except the Mobiles & Tablets and Computing category, the remaining top-performing categories (Entertainment, Appliances, and Men Fashion) demonstrated their highest sales performance during Q2 2022. This synchronized surge across multiple categories during Q2 strongly suggests that it was driven by major seasonal events, targeted promotional campaigns, or broader market trends that significantly boosted consumer spending during that period

**Recommendations**:
- Conduct comprehensive research and analysis into market trends, customer preferences, and behavior, particularly focusing on how these factors fluctuate between peak and low seasons. Utilize these insights to develop a robust strategic marketing plan aimed at sustaining high sales performance during peak periods and effectively mitigating sharp declines during low seasons
- Implement proactive sales optimization strategies specifically targeting low seasons. This includes executing timely promotions, engaging events, or offering attractive vouchers to stimulate demand and boost sales when natural momentum is lower
- Evaluate and adapt successful marketing strategies from peak seasons for application during low seasons. This approach seeks to leverage proven methodologies to drive performance even during challenging periods
- Maintain continuous vigilance on evolving market trends, technological advancements, and shifts in consumer preferences. This proactive monitoring is crucial for adapting strategies and ensuring sustained high sales performance, particularly for high-contributing categoriesMaintain high sales performance by keep observe and the market trend and lastest update of trend

#### Demand Forecasting:
- Select 3-5 of the most important products (sku_name) (e.g., best-selling or most profitable).
- Use forecasting features in Excel/Spreadsheets (e.g., Forecast Sheet or FORECAST.ETS) to predict the sales quantity for these products for the next 3-6 months.
- **Question**: Based on demand forecasts, what is the estimated stock requirement for these products in the coming months to avoid overstock or stock-out?

**Insights**:
- IDROIX_BALRX7-Gold is predicted to continue dominating the smartphone market, with estimated sales ranging from $714 million to $897 million per month over the next six months of 2023. Its total projected worth for this period is approximately $4.8 billion. This explosive growth is likely attributable to its competitive pricing (mid-range) combined with its incorporation of the latest advanced technologies, making it a highly attractive and in-demand product
- Alongside IDROIX_BALRX7-Gold, the Samsung_40K5000 is forecasted to maintain a strong presence, with a total projected worth of around $301 million over the next six months. Monthly sales are estimated to be between $45 million and $55 million, indicating its continued performance is driven by appealing features and its position as a newer model in the LED TV category.
- While iPhone 6S Plus 16GB Silver considered outdated, this model is still expected to have good sales in the first half of 2023, with a projection of $8.4 million to $10.9 million per month. Unlike the other top performers, its sales are predicted to decrease over the coming months
- Both the Samsung Galaxy S-7 and iPhone SE-16GB are projected to experience a significant sales decline, suggesting they are nearing the end of their product lifecycle. This trend is likely due to the continuous introduction of newer models with more advanced features that better suit evolving customer preferences
  
**Recommendations**:
- While IDROIX_BALRX7-Gold is projected to be the highest sales contributor in the first half of 2023, a significant restock of 900 to 1,000 units is warranted. However, its sales were heavily concentrated in Q3 2022, so ongoing analysis of market trends is crucial to avoid overstocking and ensure efficient capital utilization.
- Although the Samsung_40K5000 showed high sales performance in terms of total value in 2022 (approximately $602 million) from a very limited volume of units (21 units in total), projections for the next six months in 2023 indicate a very low total unit sales volume (around 9-11 units total). Given this, large-scale restocking is strongly discouraged. However, to anticipate potential unexpected demand surges due to specific seasonal events or market trends, a minimal restocking (for instance, around 14-15 units) can be considered. Any restocking decision must be based on thorough deep market research, analysis of current seasonal trends, and a specific evaluation of customer behavior to assess any residual or specialized demand. Prioritize selling existing units first
- Even though iPhone 6S Plus 16GB Silver is still projected to contribute the good sales, Due to its declining sales and low historical volume, high-volume restocking should be avoided. The total projected sales for the next six months equal the price of a single unit, which could be taken as the maximum quantity to restock to meet any residual demand.
- Even as top-selling items decline in general market appeal, there remains a potential opportunity to sell off existing inventory of these legacy products to price-sensitive customer segments who may not prioritize the latest models or features. It is crucial to avoid to restock these items in bulk. Develop and implement a strategic marketing plan specifically targeting these segments with appropriate pricing, bundling, or promotional offers to optimize the sales of remaining stock over the next six months without incurring losses from obsolete inventory

#### COGS (Cost of Goods Sold) Analysis and Implications:
- Analyze the trend of COGS per unit for key products (if COGS in the column is total, you need to calculate COGS per unit).
- **Question**: Is there significant variation in COGS over time or across products? How do these COGS fluctuations affect Gross Profit Margin and pricing strategies?

<img width="1009" height="282" alt="image" src="https://github.com/user-attachments/assets/daa25b60-c4b6-4396-b435-daf9b1e7452f" />

**Insights**:
- The Cost of Goods Sold (COGS) remained consistent without significant variation across the period of 2021 to 2022
- Consequently, the Gross Profit Margin (GPM) for these products remained relatively stable or stagnant throughout the same period
- Any minor observed decreases in GPM are likely attributable to the application of discounts or promotional activities, rather than fluctuations in the inherent cost of goods
  
**Recommendations**:
- Regularly analyze both the Cost of Goods Sold (COGS) and pricing strategies to ensure that the GPM remains at an optimal level for each product
- Since COGS has been stable, the primary levers for GPM optimization will be pricing adjustments and strategic promotional planning that doesn't erode profitability
- Actively seek opportunities to enhance efficiency in the supply chain or negotiate better terms with suppliers to explore potential for further profit growth

