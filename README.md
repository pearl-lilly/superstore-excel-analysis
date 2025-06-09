# Superstore-Excel-Analysis
## Introduction
This analysis investigates the superstore dataset to evaluate sales performance, profitability, and losses across different product categories and regions. The objective is to extract actionable insights by examining key metrics such as revenue, profit, losses, sales distribution, and temporal sales patterns. The finding will inform strategic decision aimed at marketing efforts, and improving regional operation to drive overall business performance.
## Project Dashboard ![Dashboard](https://github.com/user-attachments/assets/b8caefff-65d8-4445-97d2-8bd37ac4035f)

## Business Questions Addressed
To understand sales, profits, and losses across categories and regions in the Superstore dataset, I focused on the following questions:
1. **What has been the trend in profit by year, and how can it inform future planning?**  
2. **Which categories are generating losses, and what strategies can mitigate these losses?**  
3. **How do sales vary across different sub-categories, and which segments drive the most revenue?**  
4. **What is the regional distribution of sales, and which regions offer the greatest growth potential?**  
5. **Who are the top 5 customers, and how can we enhance relationships with them?**  
6. **How do sales fluctuate by month, and what seasonal trends should be considered for inventory and marketing?**
   
## Excel Skills Used
The following Excel skills were utilized for this analysis:
- **Pivot Tables**  
- **Pivot Charts**  
- **IF and TEXT functions**  
- **Data Cleaning**  
- **Use of Slicers**  
- **Date Functions (e.g., MONTH, YEAR)**  
- **Advanced Filter**  

### 📊 Dataset Source The dataset used for this project was obtained from Kaggle:  
🔗 [Superstore Dataset on Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
The dataset used for this project is the “Superstore Sales Dataset”, a real-world retail dataset available on Kaggle. It contains detailed transaction-level sales records across multiple regions and product categories.
This dataset is widely used in data analysis and visualization projects, offering a solid foundation for practicing Excel-based business analytics.
It includes information on:
	•	🗓 Order and Ship Dates
	•	📦 Product Names, Categories, and Subcategories
	•	📍 Regions and Customer Locations
	•	📈 Sales, Profit, Quantity, and Discount
	•	👤 Customer and Segment Data
## Q1.  What has been the trend in profit by year, and how can it inform future financial planning?
### Skill Used: Pivot Table and Pivot Chart
### Method:
Firstly, my order date was saved as text, so I converted it to a proper date format using the Text to Columns feature and changing the date format. Then, I created a new column named Order Year by extracting the year from the order date using the formula =TEXT([Order Date], "yyyy"). After preparing the data, I created a Pivot Table to summarize profit by subcategory for each year. Finally, I used a bar Pivot Chart to visualize the yearly profit trends clearly.
### Analysis
 ### 💡 Insights
- **2014** recorded the highest profit compared to all other years, showing it was the most successful year financially.  
- Across all years, the **Technology** category consistently generated the highest profit among all product categories.  
- This suggests that Technology products are a key driver of overall profitability and should be a focus area for the business.

### 🤔 So What

Knowing that **2014** had the highest profit helps the business understand what factors contributed to that success and consider how to replicate them in future years.  
The consistent strong performance of the **Technology** category highlights it as a valuable revenue source, suggesting the business should prioritize investment and marketing efforts in this area to maximize profits going forward.

-<a href="https://github.com/pearl-lilly/superstore-excel-analysis/blob/main/profit%20by%20year.png"> Profit By Year Chart</a>
  
## Q2 Which subcategories are generating losses, and what strategies can mitigate these losses?
### SkillUsed: Advanced Filter, Pivot Table
### Method:
I used Advanced Filter in Excel to isolate rows where the profit was less than 0, identifying only the loss-making transactions. Then, I created a Pivot Table to summarize total losses by subcategory. This helped me clearly see which subcategories were contributing to negative profit.
### Analysis
### 💡 Insights

- The total loss across all subcategories was **–$156,131**.  
- The top subcategories contributing to this loss were:  
  - **Binders:** –$38,510  
  - **Tables:** –$32,412  
  - **Machines:** –$30,119  
  - **Bookcases:** –$12,152  
  - **Chairs:** –$9,881  

Chairs, despite high sales, still resulted in a loss, highlighting that strong sales don’t always translate to profitability.  
High discount rates were a major factor driving losses in these categories.
### 🤔 So What
This analysis shows that high discounts are a key reason for the losses. The business needs to review its discount strategy, either by:
- Reducing unnecessary discounts  
- Focusing promotions on higher-margin items  
For subcategories like **Chairs**, where sales are strong but profits are low, improving pricing or cost efficiency could turn losses into gains. This insight can help protect and even improve profitability moving forward.
<a href="https://github.com/pearl-lilly/superstore-excel-analysis/blob/main/losses%20by%20sub-category.png">Losses By Sub-Category Chart</a>

## Q3.How do sales vary across different subcategories, and which segments drive the most revenue?
### Skill Used: Pivot Table, Pivot Chart
### Method:
I created a Pivot Table with Sub-Category in the Rows area and Sales in the Values area to calculate total sales by subcategory.
Then I used a Pivot Chart (Funnel chart) to visually compare sales across subcategories, making it easier to identify the highest and lowest performing segments.
### Analysis
### 💡 Insights
- The total sales across all subcategories was **$2,297,201**.  
- The top 4 subcategories by sales were:  
  - **Phones** – $330,007  
  - **Chairs** – $328,449  
  - **Copiers** – $223,844  
- These top performers accounted for a large portion of the total revenue.  
- Subcategories like **Fasteners** and **Labels** generated the least revenue, contributing very little to total sales.

### 🤔 So What
Understanding which subcategories drive the most sales helps the business focus resources where they matter most. Subcategories like **Phones**, **Chairs**, and **Copiers** are key revenue drivers and can be prioritized for:
- Inventory restocking  
- Targeted marketing campaigns  
- Sales promotions  
Meanwhile, lower-performing subcategories like **Fasteners** and **Labels** may need:
- A new marketing approach  
- Better product placement  
- Or even review for discontinuation if they’re not profitable  

This analysis supports data-driven decisions that can increase overall revenue and operational efficiency.

<a href="https://github.com/pearl-lilly/superstore-excel-analysis/blob/main/sales%20by%20sub-category.png">Sales By Sub-Category Chart</a>

## Q4. What is the regional distribution of sales, and which regions offer the greatest growth potential?
### Skill Used: Pivot Table, Pivot Chart
### Method
I created a Pivot Table with Region in the Rows area and Sales in the Values area to calculate total sales by region.
Then I used a Pivot Chart (column chart) to visually compare sales across the four regions
### Analysis
### 💡 Insights
- **West** had the highest sales at **$725,458**, showing strong performance and customer demand.  
- **East** followed closely with **$678,781**, also indicating solid sales activity.  
- **Central** recorded **$501,240**, showing moderate performance.  
- **South** had the lowest sales, at **$391,722**, despite offering the same product categories.
Sales are unevenly distributed, with the West and East regions leading in revenue.

### 🤔 So What
- The company should **maintain momentum** in the **West and East**, as they are top-performing markets.  
- The **South region** presents a clear growth opportunity. With improved marketing, localized campaigns, and better distribution, sales in this region could rise significantly.  
- The **Central region**, with moderate sales, could benefit from **targeted promotions** to push it closer to top-tier performance.
> This insight allows for data-driven regional strategy planning, optimizing resources for both immediate wins and long-term growth.
 <a href="https://github.com/pearl-lilly/superstore-excel-analysis/blob/main/sales%20by%20region.png">Sales By Region Chart</a>
 
## Q5 Who are the top 5 most profitable customers, and how can we enhance relationships with them?

### Skill Used: Pivot Table, Pivot Chart
### Method
I created a Pivot Table using Customer Name in the Rows area and Profit in the Values area.
I then sorted the Pivot Table from largest to smallest profit to identify the top 5 most profitable customers.
Finally, I visualized the result using a Pivot Chart (bar chart) to clearly highlight the highest-value customers.
## Analysis
### 💡 Insights
The top 5 most profitable customers are:  
1. **Tamara Chand** – $8,981  
2. **Raymond Buch** – $6,976  
3. **Sanjit Chand** – $5,757  
4. **Hunter Lopez** – $5,622  
5. **Adria Barton** – $5,445  
These customers have consistently purchased high-profit items and likely represent loyal or bulk buyers.
### 🤔 So What
Knowing your top customers helps shape customer retention strategies. Here’s how the company can strengthen relationships and grow profit further:
- Offer loyalty perks (e.g., exclusive discounts, early access to sales)  
- Personalize communication based on past purchases  
- Invite them to VIP programs or feedback loops to deepen engagement  
- Use their buying behavior to create customer personas for similar high-value prospects  
Focusing on these customers ensures repeat business, builds brand loyalty, and drives sustained profitability.
<a href="https://github.com/pearl-lilly/superstore-excel-analysis/blob/main/top%205%20customer%20profit.png"> Top 5 Customers Chart</a>

## Q6 How do sales fluctuate by month, and what seasonal trends should be considered for inventory and marketing?
### Skill Used: Pivot Table, Pivot Chart, Date Formatting
### Method
I first extracted the month from the Order Date column using Excel’s TEXT function:
=TEXT(Order Date, "mmm") to get the month abbreviation.
Next, I created a Pivot Table with the Month as Rows and Sum of Sales as Values.
I then sorted the months based on total sales to identify sales peaks and lows, and used a bar chart to visualize the monthly trend.
### 💡 Insights
- September had the highest sales: **$186,130.37**  
- Followed by December: **$180,432.63** and November: **$166,936.41**  
- The lowest sales occurred in February: **$34,046.84**, and January: **$50,718.98**  
This indicates that **Q4 (Sept–Dec)** is the strongest sales period, likely driven by holiday shopping, end-of-year sales, or Black Friday/Cyber Monday events.

### 🤔 So What
Understanding these seasonal patterns helps with planning inventory and marketing strategies:
- Stock up on high-demand items before September–December  
- Launch campaigns in August to build momentum into Q4  
- Use flash sales or loyalty promotions in low-sales months (e.g., Jan–Feb) to boost engagement  
- Align your marketing budget and ad spend with peak seasons to maximize ROI  
This insight supports data-driven inventory decisions and smarter promotional timing.

<a href="https://github.com/pearl-lilly/superstore-excel-analysis/blob/main/sales%20by%20month.png"> Sales By Month Chart</a>

### ✅ Conclusion
This Excel-based analysis provided clear insights into profit trends, customer behavior, subcategory performance, regional sales patterns, and monthly sales fluctuations using practical Excel tools like Pivot Tables, Advanced Filters, and IF functions.
Key takeaways include:
	•	2014 was the most profitable year, with Technology consistently leading in all categories.
	•	Subcategories like Machines, Bookcases, and Chairs experienced losses due to high discounts, indicating a need to review pricing strategies.
	•	Top-performing customers like Tamara Chand and Raymond Buch present an opportunity for loyalty programs and personalized engagement.
	•	The West and East regions drive the most revenue, but Central and South show potential for growth.
	•	Sales peak from September to December, highlighting the importance of seasonal inventory and marketing alignment.
Overall, this project shows how Excel can be used to make informed business decisions and guide strategic planning in sales, marketing, and customer management.



