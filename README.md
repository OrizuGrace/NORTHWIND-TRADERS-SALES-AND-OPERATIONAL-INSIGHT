# NORTHWIND-TRADERS-SALES-AND-OPERATIONAL-INSIGHT

##  Dataset Overview and Structure
Northwind Traders recorded a total revenue of $1.27M, showing a 1.47% Month-over-Month (MoM) increase. Gross revenue surged by 8.58%, indicating improved profitability. With 830 orders, total sales volume also rose by 1.72%, though the Average Order Value slightly dipped by 0.24%, suggesting either smaller orders or more discounts.
* Top-performing category: Beverages ($267K).
* Top customer: Horst Kloss ($110K).
* Best product: Côte de Blaye ($141K).
* Leading employee: Margaret Peacock ($232K).
* Most used shipper: United Package ($533K)
### Fact Table:
*	Sales: Order ID, Customer ID, Product ID, Employee ID, Order Date, Ship Date, Quantity, Unit Price, Total Revenue, etc.
*	Dimension Tables:
*	Customers: Company Name, Contact, Country, City, etc.
*	Products: Product Name, Category, Supplier, Unit Price, Discontinued
*	Employees: Employee Name, Region, Title
*	Shipping: Shipper ID, Company Name
*	Dates: Calendar Date, Year, Quarter, Month, Week
*	Categories: Product Category Name, Description
    * The model was structured using a Star Schema for optimized performance and intuitive relationships.
## Research Questions and Methodology
### Big Questions:
*	What are the sales trends over time?
*	Who are the top-performing customers, products, and employees?
*	Where are operational bottlenecks like delayed shipments?
*	Which products or markets are underperforming?
* How can management make data-backed decisions?
 ### Methodology:
*	Data was cleaned and modeled in Power Query using proper data types, formatting, and column splitting.
*	Star Schema modeling was applied in Power BI for clarity and performance.
*	Drill-throughs and tooltips were used to give dynamic interactivity.
*	DAX measures were created to calculate KPIs like:
       *	Total Revenue
       *	MoM Growth
       *	Avg Order Value
       *	Delay Rates

## KEY INSIGHTS, FINDING & RECOMMENDATIONS
 ### SALES PERFORMANCE
The dashboard presents a comprehensive overview of Northwind Traders' sales metrics. Key performance indicators (KPIs) include Total Revenue, Gross Revenue, Total Orders, and Average Order Value, all tracked with Month-over-Month (MoM) comparisons.
*	Total Revenue: $1.27M (▲1.47%)
*	Gross Revenue: $1.35M (▲8.58%)
*	Total Orders: 830 (▲1.72%)
*	Average Order Value: 1525 (▼0.24%)
    * A line chart shows revenue trends across months, with a noticeable dip mid-year (May-June) followed by a gradual recovery.

## CUSTOMER BEHAVIOUR
* Northwind Traders serves 91 customers, with an impressive 97% returning customer rate (88 out of 91).
* The average revenue per customer is $13.91K, while the Customer Lifetime Value (CLV) totals $1.27M.
* The Retention Rate showed stability from July to December, while the Churn Rate declined.
* Top revenue is driven by Loyal Customers ($598K) and Champions ($421K).
* Horst Kloss leads with $110K in revenue from 28 orders, boasting the highest AOV ($3938).

## Strategic Recommendations
1.	Replicate July-December retention strategies across other months.
2.	Build stronger relationships with the top 5 revenue customers.
3.	Introduce tiered rewards for Champions and Loyal Customers.
4.	Upsell opportunities: Explore product bundling for customers with lower AOV.
5.	Keep monitoring churn early in the year, as January–June showed higher risk.

## PRODUCT INSIGHTS
Key Metrics
*	Total Product Sold: 4 million units
*	Best Selling Product: Côte de Blaye ($141.4K in revenue)
*	Average Revenue Per Product: $16.44K
*	Discontinued Products: 10.39%
  
 ## Revenue Insights
*	Top Products by Revenue:
   * o	Côte de Blaye leads by a significant margin.
   * o	Other strong performers: Thüringer Rostbratwurst, Raclette Courdavault.
*	Revenue vs. Units Sold:
   * o	Scatter plot shows some products with high sales volume but lower revenue, hinting at low unit prices or heavy discounts.
* Discount Impact
   * o	Dairy Products ($8.60K)
   * o	Beverages ($8.59K)
   * o	Meat & Poultry ($7.37K)
*	Discounts are heavily affecting profit margins in key categories.
   * Category Summary
   * o	Beverages, Dairy Products, and Meat & Poultry lead.
   * o	Discrepancies between gross and net revenue indicate areas of discount leakage.

 Recommendations
1.	Review pricing and discount policies for top loss categories (Dairy, Beverages).
2.	Promote high-revenue products with low discount impact (like Côte de Blaye).
3.	Drill into discontinued products to understand why they were pulled and if there’s potential for revival.
4.	Utilize tooltip and drill-through functionality to allow deeper product- and category-level exploration during executive reviews.

 Shipping & Delivery
•	Top Metrics Overview
•	Total Freight Cost: $64.94K
•	Average Delivery Time: 8 days
•	Total Late Shipments: 37
•	On-Time Delivery Rate: 98.02%
•	 Insight:
You're operating at a very high delivery performance rate with only 1.98% of shipments late. This is exceptional in logistics—shows strong operational efficiency.
Delivery time is relatively consistent across countries, but Ireland stands out as being slower by 2 days. This could be due to distance, customs, or internal processing delays. Worth investigating further.
United Package generates the highest revenue, suggesting it handles either high-volume or high-value shipments. It might be your primary logistics partner—evaluate their cost-benefit performance closely.
High order density in:
o	USA
o	Brazil
o	Germany
o	France
o	Australia
These countries are your key markets for order volume. Strategically, consider setting up fulfillment centers or improving warehousing near these regions for even faster delivery.

 Recommendations
1.	Investigate Ireland's delivery delays—see if a new carrier or route can reduce the average.
2.	Audit United Package's delivery issues despite their high volume. Can performance improve further?
3.	Leverage Federal Shipping's efficiency more if cost-effective.
4.	Use volume data to optimize regional warehousing or fulfillment partnerships.
5.	Maintain the 98% on-time rate—it's a massive trust factor for customer satisfaction and loyalty.

Employee Insights
🔹 Key Highlights
•	Number of Employees: 9
•	Top Employee: Margaret Peacock
•	Revenue per Employee: $140.64K
•	Average Order Value (AOV): $1.53K

🔹 Top Performers
•	Margaret Peacock leads with:
o	75 customers
o	$232.9K in revenue
o	AOV of $1,493
•	Janet Leverling and Nancy Davolio follow closely behind with revenues of $202.8K and $192.1K, respectively.
•	All top 3 employees are based in the USA.
🔹 Country-Based Insight
•	USA-based employees dominate the top rankings.
•	UK-based employees are currently underperforming in comparison, suggesting an area for growth or support.
🔹 Revenue Trends (Monthly)
•	April shows the highest spike across multiple employees, notably:
o	Andrew Fuller: $44.1K
o	Anne Dodsworth: $100.66K
•	Some employees, such as Steven Buchanan, show inconsistent monthly performance—potentially due to seasonal demand or account assignments.

 Recommendations
1.	Reward high performers like Margaret Peacock to retain top talent.
2.	Coach underperforming employees, particularly in the UK.
3.	Analyze April's spike to identify what drove high revenue — campaigns, promotions, or customer onboarding.
4.	Track AOV changes over time to ensure sales quality is maintained, not just volume.



