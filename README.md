📦 SUPPLY CHAIN ANALYSIS PROJECT
(EDA + Power BI Dashboard)


🧠 Project Overview

This project analyzes Supply Chain performance data to understand how delivery delay time, cost, region, and stage affect overall efficiency.

The work was done in two main parts:
1️. Exploratory Data Analysis (EDA) using Python
2️. Dashboard Creation using Power BI

The goal was to find what causes high delay times and high delivery costs — and use data to suggest ways to improve supply chain performance.


🧾 Dataset Description

Source: Kaggle
Rows: 1,000+ records (as used in this project)
Columns: 16

Key Columns Used:

- Transaction_ID
- Route_ID
- Stage (Manufacturing, Warehouse, Logistics, Retailer)
- Entity
- Timestamp
- RFID_ID
- Region (Urban / Rural)
- Speed
- Delay_Time
- Cost
- Temperature
- Humidity
- Delivery_Status (Completed / In Transit)

Each record represents one delivery transaction in the supply chain.


🧮 Exploratory Data Analysis (EDA) — Python

🔹 Tools Used

Tool	                           Purpose

Python	                           For data analysis and exploration
Pandas	                           Data cleaning, grouping, and summary calculations
Matplotlib & Seaborn	           Visualizations (bar, line, scatter, pie)
Jupyter Notebook	               Running and visualizing analysis results

🔹 EDA Steps Performed

1. Data Cleaning

     -Checked for missing and duplicate values
     -Verified data types for all columns
     -Removed inconsistencies in region and stage labels

2. Exploration

     - Counted deliveries by stage, region, and entity
     -Calculated average delay time and average cost
     -Identified top 10 routes with longest average delays
     -Found top entities with lowest delivery costs
     -Compared Urban vs Rural performance
     -Checked if temperature or humidity affected delays

3. Statistical Insights

     -Compared each delivery stage (Manufacturing, Warehouse, Logistics, Retailer)
     -Calculated average delay and cost for each region
     - Explored relationships between Speed vs Delay Time, Cost vs Delay, etc.

🔹 Key Findings from EDA

1. Stage-wise Insights:

    -Logistics stage had the highest average delay time.
    -Warehouse also showed frequent moderate delays.    
    -Manufacturing and Retailer stages were more stable.

2.  Region-wise Insights:

    -Rural regions showed higher delay time and cost.
    -Urban regions were faster and more consistent.

3. Route Insights:

    -Certain routes repeatedly had the longest average delays — indicating route inefficiency.
    -Top 10 delayed routes were identified for improvement.

4. Entity Insights:

    -Some entities like Supplier A and Carrier B had the most disruptions.
    -Entities such as Warehouse C maintained lower average costs — showing operational efficiency.

5. Other Observations:

    -Speed and Delay Time showed no strong relationship — faster speed didn’t always mean fewer delays.
    -Temperature and Humidity had minor effect on delay time and cost.

📊 Power BI Dashboard

After completing EDA in Python, an interactive Power BI Dashboard was created to visualize all findings and help businesses quickly identify performance problems.


🔹 Tools Used

Tool	                    Purpose

Power BI	                Dashboard creation and visualization
Python (EDA phase)	        For data preparation and insights
Excel	                    For dataset preview and upload
VS Code	                    Editing and documentation


🧩 Dashboard Structure (4 Pages Total)

🔸 Page 1 – Delivery Performance Overview

This page gives a full summary of delivery efficiency across all supply chain stages.

Includes:

    -KPIs: Total Transactions (1K), Total Cost ($269K), Average Delay Time (23.15 hrs), and Delivery % (52%)

    -Donut Chart: Delivery Status (Delivered vs In Transit)

    -Bar Chart: “Which Stage Has the Most Delays?” (Retailer slightly highest, then Warehouse, Manufacturing, and Logistics)

    -Line Chart: “How Are Delays Changing Over Time?” — delay time gradually decreases from August to December

    -Filters: Stage, Partner, and Issue Type

Insights:

    • Retailer stage records the highest average delay time (23.59 hrs), though all stages are close.

    • Overall delay trend decreases over the months, showing improvement in performance.

    • Delivery completion rate is around 52%, suggesting room for process optimization.

🔸 Page 2 – Risk & Disruption Analysis

This dashboard focuses on risk types, their frequency, and how they impact delivery performance.

Includes:

    -KPIs: Total Disruptions (1K), Average Delay (Top Risk = 23.95 hrs)

    -Bar Chart: “What Types of Risks Occur Most?” (Traffic and Weather are top causes)

    -Bar Chart: “Which Risks Cause the Biggest Delays?” — Equipment Failure has the highest average delay

    -Table: “Top Routes Facing Biggest Delays” (e.g., Route_177, Route_316, Route_456)

    -Stacked Chart: “How Issues Affect Delivery Status” (Delivered vs In Transit by risk type)

    -Cards: Top Risk Factor (Traffic) and Most Affected Stage (Retailer)

    -Filter Panel: Risk-based filtering (Traffic, Human Error, Equipment Failure, Weather)

Insights:

    • Traffic is the most frequent risk factor, while Equipment Failure causes the longest delays.

    • Retailer stage faces the most disruptions.

    • Weather-related delays are also significant but not the highest.

🔸 Page 3 – Cost and Efficiency Insights

This page analyzes cost distribution and partner performance across routes, regions, and stages.

Includes:

    -KPIs: Avg Cost per Delivery ($269), Highest Cost Route (Route_621)

    -Pie Chart: “Which Region Has the Highest Delivery Cost?” — Urban region dominates with 86% of total cost

    -Bar Chart: “Which Partners Have the Highest Delivery Cost?” (Carrier B, Supplier A, and Warehouse C are top three)

    -Table: “Top Routes That Cost the Most” — includes multiple routes handled by different entities

    -Bar Chart: “Delivery Results Across Each Stage” (Delivered vs In Transit %)

    -Line Chart: “Total Transactions per Month” showing fluctuations across the year

Insights:

    • Carrier B and Supplier A handle the costliest deliveries.

    • Urban deliveries contribute to the majority of total cost.

    • Warehouse stage has slightly more successful deliveries (56%).

    • Total transactions fluctuate, peaking at 99 per month.

🔸 Page 4 – Environmental & GPS Tracking

This dashboard studies how temperature, humidity, and speed affect delivery delay and stage performance.

Includes:

    -KPIs: Average Temperature (17.07°C), Average Humidity (50%), Average Speed (54.86 km/h)

    -Dual Line Chart: “How Do Temperature and Humidity Change Over Time?” (over several months)

    -Bar Chart: “Which Stage Has the Highest Average Speed?” — Manufacturing is fastest (57 km/h)

    -Combo Chart: “How Do Speed and Delay Change Across Stages?” showing both speed and average delay

Insights:

    • Manufacturing stage has the highest average speed (57 km/h).

    • Retailer stage has lowest speed (53 km/h) but highest delay (23.59 hrs).

    • Environmental factors (temperature & humidity) fluctuate but have minimal effect on delays.


💡 Key Insights Summary

Category	              Findings

Stage	                  Logistics & Warehouse cause most delays
Region	                  Rural areas have higher delay & cost
Route	                  Few routes are consistently slow — need optimization
Entity	                  Some entities manage cost efficiently; others face frequent disruptions
Speed	                  No clear link between speed and delay time
Weather	                  Minor effect on delivery performance


🎯 Business Impact

This analysis helps businesses pinpoint where time and money are being lost.
By improving the Logistics and Warehouse stages and optimizing underperforming routes, organizations can:

-Reduce delivery delays

-Cut transportation and logistics costs

-Improve supply chain planning and coordination

-Use data-driven insights for faster decision-making


✨ Final Conclusion

This project demonstrates how data analysis and visualization can reveal deep insights into supply chain efficiency.
Using Python for EDA and Power BI for dashboarding, raw data was turned into clear, actionable insights.

Key takeaway:
Delays are mainly caused by Logistics inefficiency and regional challenges, not by speed or weather.
Targeting these problem areas can greatly improve delivery time and cost performance.

