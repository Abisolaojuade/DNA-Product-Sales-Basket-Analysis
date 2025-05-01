# DNA project sales Analysis

![Product image](https://github.com/user-attachments/assets/bd34ff58-42b7-462b-8b36-d62ee7e4099e)


## Table of Contents

- [Introduction](#Introduction)
- [Dataset Overview](#Dataset-Overview)
- [Project Objective](#Project-Objective)
- [Data Cleaning and Transformation](#Data-Cleaning-and-Transformation)
- [Data Exploration and Insights](#Data-Exploration-and-Insights)
- [Dashboard](#Dashboard)
- [Recommendation](#Recommendation)
- [Conclusion](#Conclusion)

## Introduction

This project involves analyzing product sales data to uncover business insights, understand customer buying behavior, and forecast future performance. 
Using a CSV file containing detailed sales records—including customer information, order ID, order date, purchase address, product names, quantity ordered, 
and sales price—I performed a comprehensive analysis entirely in **Power BI**.
Key objectives of the project included:
- Identifying top-selling products and regions  
- Performing basket analysis to discover product combinations frequently bought together  
- Visualizing sales trends and performance metrics  
- Setting informed sales targets based on historical data  
- Forecasting future sales using Power BI's built-in analytics tools  
The result is an interactive Power BI dashboard that enables data-driven decision-making and supports strategic planning for improved sales performance.

---

## Dataset Overview

The dataset includes the following columns:

- **Order ID**: Unique number to track orders  
- **Products**: The products that have been sold  
- **Quantity Ordered**: Total item quantity ordered  
- **Price Each**: The price of each product  
- **Order Date**: Date the order is to be shipped  
- **Purchase Address**: Includes billing, shipping, and PO number details  

---

## Project Objective
The objective of this project is to analyze product sales data using Power BI in order to extract actionable insights that can drive strategic business decisions.
Key Business Questions to Solve:
1. What is the best year for sales? How much was earned that year?  
2. What was the best month for sales? How much was earned that month?  
3. Which day of the week has the best sales?  
4. What city had the highest number of sales?  
5. What time should we display advertisement to maximize likelihood of customer’s buying products?  
6. What products are most often sold together?  
7. What product sold the most? Why do you think it sold the most?  

![Screenshot 2025-04-30 160544](https://github.com/user-attachments/assets/919d82e8-3dc4-425d-8981-30b4d78a7a59)


---

## Data Cleaning and transformation

Performed in Power BI using Power Query:

- **Duplicate Check and Removal**
- **Date Extraction**: Month, Year, Weekday, Hour  
- **Time Grouping**: Created periods (Morning, Afternoon, Evening, Night)  
- **Sales Column Creation**: Quantity × Price  
- **Data Type Formatting**: Ensured proper formats for all columns  

---

## Data Exploration and Insights
### 1. What is the best year for sales? How much was earned that year?
**INSIGHTS:** The analysis of total sales over time revealed a significant insight into the company's yearly performance:
- Total Sales over the entire period amounted to **$34.47 million**.
- The best-performing year was **2019**, with an outstanding total of **$34,456,867.65**, accounting for nearly all recorded sales in the dataset.
- In contrast, **2020** saw a dramatic drop in revenue, generating only **$8,620**, which is less than **0.03%** of **2019’s** sales.

This drastic difference suggests that the dataset either: Covers only a limited portion of **2020**, possibly due to missing or incomplete data, 
Or that business operations were significantly disrupted in **2020** (e.g., due to external factors like the COVID-19 pandemic). 

This insight emphasizes the importance of understanding external influences on sales performance and ensuring complete data coverage for more accurate year-over-year comparisons.

### 2. What was the best month for sales?  How much was earned that month?
**INSIGHTS:** An analysis of monthly sales performance highlights **December** as the best month for sales, generating a total revenue of **$4,608,295.70.**
This peak in December sales likely reflects the impact of holiday shopping and year-end consumer spending, which are typically strong drivers of retail performance. The increase may be attributed to:
- Holiday promotions and discounts
- Increased demand for gifts and seasonal products
- End-of-year inventory clearances

This trend underscores the importance of seasonal planning in sales strategy. Businesses can capitalize on this by increasing inventory,
enhancing marketing efforts, and preparing logistics in advance of the holiday season to maximize revenue during this critical period.

### 3. Which day of the week has the best sales?
**INSIGHTS:** From the weekday analysis, **Tuesday** emerged as the day with the highest total sales, generating **$5,086,275.40.**
This insight may indicate a pattern in customer behavior or business operations, such as: Successful weekday marketing campaigns or promotions, 
Consumer preference for making online purchases early in the week, Efficient delivery or order processing systems encouraging Tuesday purchases.

### 4. What city had the highest number of sales?
**INSIGHTS:** Among all the cities analyzed, **San Francisco** recorded the highest total sales, amounting to **$8,254,743.55**.

This suggests that **San Francisco** is a key market for the company, potentially due to:
- A high concentration of target customers
- Greater purchasing power or demand for the company’s products
- Effective local marketing and distribution strategies

This insight highlights the value of geographic segmentation in sales strategy. 
Focusing on high-performing cities like San Francisco can help businesses prioritize resources, launch targeted campaigns, and explore expansion opportunities in similar urban markets.

### 5. What time should we display advertisement to maximize likelihood of customer’s buying products?
**INSIGHTS:** Analysis of sales by time of day shows that the **Evening period (6:01 PM – 9:00 PM)** is the most effective time to target customers with advertisements.
This peak buying window suggests that customers are most likely to make purchases in the evening, possibly after work hours when they are relaxed, browsing online, or engaging with digital content.
To maximize conversions, businesses should:
- Schedule digital ads and promotional content during this timeframe
- Optimize email campaigns or social media posts for evening engagement
- Ensure website and customer service responsiveness is strong during these peak hours

Leveraging this insight can significantly improve ad visibility, customer engagement, and overall sales performance.

### 6. What products are most often sold together? 
**INSIGHTS:** Using basket analysis, the top 5 product combinations that are most often purchased together were identified. 
These combinations provide insight into customer buying behavior and opportunities for cross-selling. The most frequent pairs include:
| Product Combination                  | Confidence (Prod 1) | Confidence (Prod 2) | Lift |
|-------------------------------------|---------------------|---------------------|------|
| USB-C Charging Cable & Google Phone | 4.56%               | 18.06%              | 1.47 |
| Vareebadd Phone & USB-C Cable       | 17.82%              | 1.68%               | 1.45 |
| Lightning Cable & iPhone            | 4.68%               | 14.78%              | 1.22 |
| Wired Headphones & Google Phone     | 2.24%               | 7.64%               | 0.72 |
| Wired Headphones & Vareebadd Phone  | 0.79%               | 7.22%               | 0.68 |

- A **Lift > 1** indicates a strong association between products. **The USB-C Charging Cable & Google Phone pair has the highest lift (1.47)**, 
suggesting that customers who buy a Google Phone are highly likely to also purchase a USB-C Charging Cable.

These associations can be leveraged to:
- Create product bundles or combo deals
- Offer cross-selling recommendations during checkout
- Inform inventory placement and packaging strategies

This analysis enhances marketing effectiveness by promoting relevant product pairings and improving the overall customer purchase experience.

### 7. What product sold the most? Why do you think it sold the most?
**Insights:** The **MacBook Pro Laptop** was the top-selling product, generating a total revenue of **$8,032,500**.

The strong sales performance of the MacBook Pro Laptop can be attributed to several potential factors:
- High demand for premium tech products, particularly among professionals and students
- Brand reputation and loyalty, with Apple products known for quality and ecosystem integration
- Higher price point, which naturally contributes to higher total sales revenue even with fewer units sold compared to lower-priced items
- Possible business or educational partnerships, driving bulk or recurring purchases

This insight highlights the value of tracking product-level performance to understand what drives revenue and to help shape future product strategy, marketing focus, and inventory planning.

---

## Dashboard
The image below is the Dashboard for my analysis

![DNA Product sales Dashboard_page-0001](https://github.com/user-attachments/assets/f1ad5cac-a3a9-4e04-ab70-7050a52eb5b2)


---
## Recommendation

Based on the data exploration and sales insights, the following recommendations are proposed to help the business optimize performance, boost revenue, and improve strategic decision-making:

### 1. **Capitalize on High-Sales Periods**
- **Focus marketing and inventory planning around December**, the peak sales month, by launching promotions, bundle offers, and early holiday campaigns.
- **Prepare ahead of time for seasonal demand** to avoid stockouts and maximize revenue opportunities during the year-end shopping season.

### 2. **Leverage Weekly and Hourly Buying Trends**
- **Concentrate advertisement campaigns on Tuesdays**, the highest sales day, to take advantage of increased purchasing activity.
- **Schedule digital ads and customer engagement activities during the evening hours (6:01 PM – 9:00 PM)** when customers are most likely to buy.

### 3. **Target High-Performing Locations**
- **Double down on marketing efforts in San Francisco** and similar high-performing cities with strong sales figures. Use geo-targeted ads and local partnerships to drive further growth.
- Consider **replicating strategies from San Francisco** in other regions with untapped potential.

### 4. **Promote Frequently Bought-Together Products**
- Use **basket analysis results** to implement **automated cross-sell and upsell recommendations** on product pages and at checkout.
- Introduce **product bundles** (e.g., phones with compatible accessories like charging cables or headphones) to encourage larger order sizes and improve customer convenience.

### 5. **Continue Monitoring Product Performance**
- Track top-selling products like the **MacBook Pro Laptop** to understand customer demand and pricing sensitivity.
- Use insights from high-value items to **inform product development, partnership strategies, and stocking priorities**.

### 6. **Review and Complete Data Coverage**
- Address data limitations—especially the sharp decline in 2020 sales—by **verifying dataset completeness** and **ensuring consistent data collection moving forward**.
- Consider **integrating other data sources** (e.g., marketing, customer demographics, or supply chain data) for a more holistic view of business performance.

---

## Conclusion
The DNA Product Sales Analysis project successfully leveraged Power BI to uncover meaningful insights from sales transaction data, enabling data-driven decision-making.
Through detailed trend analysis, basket analysis, and time-based segmentation, the report identified key patterns in customer behavior, product performance, and regional sales distribution.

The analysis highlighted significant business opportunities:
- December is the most profitable month, emphasizing the importance of seasonal sales strategy.
- Tuesday evenings present the best window for customer engagement.
- San Francisco stands out as a top-performing city, offering a strong regional growth opportunity.
- Frequently bought-together items present clear opportunities for cross-selling and bundling strategies.
- The MacBook Pro Laptop leads in sales, underscoring the value of premium product offerings.

By transforming raw data into a dynamic Power BI dashboard, the project not only provided answers to critical business questions but also delivered a visual tool for continuous monitoring and strategic planning. 
This dashboard can be used by stakeholders across departments—from marketing to operations—to guide smarter decisions, optimize campaigns, and drive sustained revenue growth.
