# FLUXX LOGISTICS PERFORMANCE REPORT

**Live Interactive Dashboard**: https://shorturl.at/VsCur

**Project Video**: https://shorturl.at/2npc6

## PROBLEM STATEMENT

As Fluxx Logistics approaches its two-year anniversary since commencing operations in August 2022, the company seeks to optimize its supply chain efficiency and  maintain a competitive edge in the market. To achieve this, Fluxx Logistics needs to identify areas of improvement. Through in-depth data analysis, the company aims to:

- **Enhance operational efficiency** by reducing average delivery time and increasing on-time delivery rates.
- **Maximize revenue potential** by identifying top-performing sales teams, regions, and product categories.
- **Inform data-driven decisions** to drive business growth and stay competitive in the logistics industry.

## DATA
For this analysis, the following tables were used:

- **Country**: Lists countries and regions.
- **Product**: Contains product names, categories, and cost per unit.
- **Shipment**: Tracks shipment ID, salesperson, country, product, dispatch date, sales, status, delivery date, and delivery duration.
- **Sales Person**: Lists salespersons and their respective teams.
- **Date**: Generated from dispatch dates, including fields for year and month.

## TRANSFORMATIONS PERFORMED

- **Delivery Time Calculation**: A new column `Delivery Time` was created, calculated as `Delivery Date - Dispatch Date`.
- **Date Table Creation**: A comprehensive Date table was created using dispatch dates from the Shipment table.
- **Data Type Fixes**: Resolved an issue where changing the data type for date columns (Dispatch and Delivery Dates) caused errors. After exploring multiple methods, the `Date Locale` method provided a solution.

## METRICS
Used **DAX formula** to calculate key metrics, like:

- Completed Shipments
- Average Delivery Time
- Revenue per Shipment
- On-Time Delivery Rate
- Year-over-Year (YoY) Revenue Growth
and 15+ other metrics
<div align="center">
    <img src="https://github.com/user-attachments/assets/fdd684a0-7c5f-4acd-935c-9029569f9cd2" alt="measures">
    <img src="https://github.com/user-attachments/assets/65f701c6-a6d8-47cb-a305-2b0c70172340" alt="measures 2">
</div>

## VISUALIZATIONS
<div align="center">
    <img src="https://github.com/user-attachments/assets/3c70ef1f-5b7a-4c04-8141-eac437be8a66" alt="1">
</div>

Integrated a number of visuals:

- KPI tiles
- Table
- Waterfall chart
- Line chart
- Bar chart
- Donut chart
- Heatmap
- Gauge chart
- Tooltip
<div align="center">
    <img src="https://github.com/user-attachments/assets/ce3dce09-72c0-4be5-baeb-2103bb467a96" alt="2">
</div>
<div align="center">
    <img src="https://github.com/user-attachments/assets/7e00372b-f5d2-47de-981c-2e4de8f3c725" alt="4">
</div>

## INSIGHTS

- **Operational Efficiency**: While the overall on-time delivery rate is 75%, regions like Australia with a 20-day average delivery time indicate a need for efficiency improvements.
- **Revenue Trends**: Revenues peaked in March and May, suggesting these months are critical for business performance.
- **Salesperson Performance**: There is a significant variance in revenue generation among sales personnel, with Sandra leading at $99k and Catherine trailing at $67.21k.

## RECOMMENDATIONS

- **Optimize Delivery Times**: Focus on reducing delivery times in high-delay regions like Australia. Reevaluate and renegotiate contracts with logistics partners in these areas to improve efficiency.
- **Sales Personnel Performance Enhancement**: Introduce performance-based incentives and provide targeted training for sales personnel with lower success rates.
- **Improve On-Time Delivery Rate**: Identify and address bottlenecks causing 25% of late shipments. Implement measures to streamline processes and enhance efficiency.
- **Address Shipment Returns**: Investigate high return rates, particularly among specific sales personnel. Develop a customer feedback loop to understand and address reasons for returns, and implement corrective actions.
- **Address Revenue Discrepancies Across Countries**: Develop targeted marketing and sales strategies for underperforming regions like Brazil. Allocate additional budget to marketing and implement a flexible go-to-market strategy to adapt to market shifts.
- **Rapport Building**: Position Fluxx Logistics as a leader in sustainable logistics by setting and transparently communicating ambitious sustainability goals. This will enhance the company’s reputation and attract environmentally conscious clients.

## KEY ACHIEVEMENTS
- **Transformed reporting infrastructure** by migrating from Excel to Power BI dashboard, slashing reporting time by 30%.
  
- Uncovered growth opportunities in **high-performing products and key markets**, boosting revenue in 6 months through strategic partnerships and targeted promotions.

- Led an in-depth data analysis that achieved a **14% reduction in return rates**, a **20% enhancement in employee performance**, and **21% surge in overall revenue**.

- Optimized dashboard functionality using slicers, bookmarks, and buttons, improving **dashboard adoption rate by 12%**.

- **Automated data cleaning** using Power Query, slashing manual work from 30mins to 2min, improving efficiency by 90%.

## CHALLENGE FACED, AND SOLUTION

During the data transformation process, an issue arose when attempting to change the data type for date columns (Dispatch Date and Delivery Date). Every attempt to adjust these columns resulted in errors.

After navigating various options and researching potential fixes on the internet, I discovered the `Date Locale` method. By applying this method, I successfully resolved the issue, allowing the correct data type to be applied without errors. 
