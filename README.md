# 📦 SUPPLY CHAIN ANALYSIS PROJECT
### EDA + Power BI Dashboard

---

## 🧠 Project Overview
This project analyzes **Supply Chain performance data** to understand how delivery delay time, cost, region, and stage affect overall efficiency.

The work was done in two main parts:
1. **Exploratory Data Analysis (EDA)** using Python  
2. **Dashboard Creation** using Power BI  

🎯 The goal: find what causes high delay times and high delivery costs — and use data to suggest ways to improve supply chain performance.

---

## 🧾 Dataset Description

**Source:** Kaggle  
**Rows:** 1,000+ records  
**Columns:** 16  

**Key Columns Used:**
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

---

## 🧮 Exploratory Data Analysis (EDA) — Python

### 🔹 Tools Used
| Tool | Purpose |
|------|----------|
| **Python** | Data analysis and exploration |
| **Pandas** | Data cleaning, grouping, and summary calculations |
| **Matplotlib & Seaborn** | Visualizations (bar, line, scatter, pie) |
| **Jupyter Notebook** | Running and visualizing analysis results |

---

### 🔹 EDA Steps Performed
#### 1. Data Cleaning
- Checked for missing and duplicate values  
- Verified data types for all columns  
- Removed inconsistencies in region and stage labels  

#### 2. Data Exploration
- Counted deliveries by stage, region, and entity  
- Calculated average delay time and cost  
- Identified top 10 routes with longest delays  
- Found top entities with lowest delivery costs  
- Compared Urban vs Rural performance  
- Checked temperature and humidity effects  

#### 3. Statistical Insights
- Compared each delivery stage (Manufacturing, Warehouse, Logistics, Retailer)  
- Calculated averages by region  
- Explored relationships like Speed vs Delay Time, Cost vs Delay, etc.  

---

### 🔹 Key Findings from EDA

#### **Stage-wise Insights**
- Logistics stage had the highest average delay time.  
- Warehouse also showed moderate delays.  
- Manufacturing and Retailer stages were more stable.  

#### **Region-wise Insights**
- Rural regions showed higher delay time and cost.  
- Urban regions were faster and more consistent.  

#### **Route Insights**
- Certain routes repeatedly had the longest delays — indicating inefficiency.  
- Top 10 delayed routes were identified for improvement.  

#### **Entity Insights**
- Entities like Supplier A and Carrier B had the most disruptions.  
- Warehouse C maintained lower costs — showing efficiency.  

#### **Other Observations**
- Speed and Delay Time showed no strong relationship.  
- Temperature and Humidity had minor effects on delay and cost.  

---

## 📊 Power BI Dashboard

After completing EDA in Python, an interactive **Power BI Dashboard** was created to visualize all findings and help businesses quickly identify performance problems.

### 🔹 Tools Used
| Tool | Purpose |
|------|----------|
| **Power BI** | Dashboard creation and visualization |
| **Python** | Data preparation and insights |
| **Excel** | Dataset preview and upload |
| **VS Code** | Editing and documentation |

---

## 🧩 Dashboard Structure (4 Pages)

### 🔸 Page 1 – Delivery Performance Overview
**Includes:**
- KPIs: Total Transactions (1K), Total Cost ($269K), Avg Delay Time (23.15 hrs), Delivery % (52%)  
- Donut Chart: Delivery Status  
- Bar Chart: Delays by Stage  
- Line Chart: Delay Trend Over Time  
- Filters: Stage, Partner, Issue Type  

**Insights:**
- Retailer stage has the highest delay (23.59 hrs).  
- Delay trend decreases from Aug–Dec.  
- Delivery completion ≈ 52%.  

---

### 🔸 Page 2 – Risk & Disruption Analysis
**Includes:**
- KPIs: Total Disruptions (1K), Avg Delay (23.95 hrs)  
- Bar Charts: Risk Types, Risk Delays  
- Table: Top Delayed Routes  
- Cards: Top Risk (Traffic), Most Affected Stage (Retailer)  

**Insights:**
- Traffic is the most frequent risk.  
- Equipment Failure causes the longest delays.  
- Retailer stage faces the most disruptions.  

---

### 🔸 Page 3 – Cost and Efficiency Insights
**Includes:**
- KPIs: Avg Cost per Delivery ($269), Highest Cost Route (Route_621)  
- Pie Chart: Cost by Region  
- Bar Chart: Partner Costs  
- Table: Costliest Routes  
- Line Chart: Transactions per Month  

**Insights:**
- Carrier B and Supplier A are most costly.  
- Urban region contributes 86% of total cost.  
- Warehouse stage has most successful deliveries (56%).  

---

### 🔸 Page 4 – Environmental & GPS Tracking
**Includes:**
- KPIs: Avg Temp (17.07°C), Humidity (50%), Speed (54.86 km/h)  
- Dual Line Chart: Temperature & Humidity over Time  
- Combo Chart: Speed vs Delay by Stage  

**Insights:**
- Manufacturing is fastest (57 km/h).  
- Retailer has lowest speed but highest delay.  
- Environmental factors have minimal effect.  

---

## 💡 Key Insights Summary

| Category | Findings |
|-----------|-----------|
| **Stage** | Logistics & Warehouse cause most delays |
| **Region** | Rural areas have higher delay & cost |
| **Route** | Few routes are consistently slow |
| **Entity** | Some entities are efficient; others face disruptions |
| **Speed** | No clear link with delay |
| **Weather** | Minor impact on performance |

---

## 🎯 Business Impact
This analysis helps businesses pinpoint where time and money are being lost.

By improving the Logistics and Warehouse stages and optimizing underperforming routes, organizations can:
- Reduce delivery delays  
- Cut logistics costs  
- Improve coordination  
- Make data-driven decisions  

---

## ✨ Final Conclusion
This project demonstrates how **data analysis and visualization** reveal deep insights into supply chain efficiency.

Using **Python for EDA** and **Power BI for dashboards**, raw data was turned into actionable insights.

**Key takeaway:**  
Delays are mainly caused by **Logistics inefficiency and regional challenges**, not speed or weather.  
Targeting these areas can greatly improve delivery time and cost performance.

**Rows:** 1,000+ records  
**Columns:** 16  

**Key Columns Used:**
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

---

## 🧮 Exploratory Data Analysis (EDA) — Python

### 🔹 Tools Used
| Tool | Purpose |
|------|----------|
| **Python** | Data analysis and exploration |
| **Pandas** | Data cleaning, grouping, and summary calculations |
| **Matplotlib & Seaborn** | Visualizations (bar, line, scatter, pie) |
| **Jupyter Notebook** | Running and visualizing analysis results |

---

### 🔹 EDA Steps Performed
#### 1. Data Cleaning
- Checked for missing and duplicate values  
- Verified data types for all columns  
- Removed inconsistencies in region and stage labels  

#### 2. Data Exploration
- Counted deliveries by stage, region, and entity  
- Calculated average delay time and cost  
- Identified top 10 routes with longest delays  
- Found top entities with lowest delivery costs  
- Compared Urban vs Rural performance  
- Checked temperature and humidity effects  

#### 3. Statistical Insights
- Compared each delivery stage (Manufacturing, Warehouse, Logistics, Retailer)  
- Calculated averages by region  
- Explored relationships like Speed vs Delay Time, Cost vs Delay, etc.  

---

### 🔹 Key Findings from EDA

#### **Stage-wise Insights**
- Logistics stage had the highest average delay time.  
- Warehouse also showed moderate delays.  
- Manufacturing and Retailer stages were more stable.  

#### **Region-wise Insights**
- Rural regions showed higher delay time and cost.  
- Urban regions were faster and more consistent.  

#### **Route Insights**
- Certain routes repeatedly had the longest delays — indicating inefficiency.  
- Top 10 delayed routes were identified for improvement.  

#### **Entity Insights**
- Entities like Supplier A and Carrier B had the most disruptions.  
- Warehouse C maintained lower costs — showing efficiency.  

#### **Other Observations**
- Speed and Delay Time showed no strong relationship.  
- Temperature and Humidity had minor effects on delay and cost.  

---

## 📊 Power BI Dashboard

After completing EDA in Python, an interactive **Power BI Dashboard** was created to visualize all findings and help businesses quickly identify performance problems.

### 🔹 Tools Used
| Tool | Purpose |
|------|----------|
| **Power BI** | Dashboard creation and visualization |
| **Python** | Data preparation and insights |
| **Excel** | Dataset preview and upload |
| **VS Code** | Editing and documentation |

---

## 🧩 Dashboard Structure (4 Pages)

### 🔸 Page 1 – Delivery Performance Overview
**Includes:**
- KPIs: Total Transactions (1K), Total Cost ($269K), Avg Delay Time (23.15 hrs), Delivery % (52%)  
- Donut Chart: Delivery Status  
- Bar Chart: Delays by Stage  
- Line Chart: Delay Trend Over Time  
- Filters: Stage, Partner, Issue Type  

**Insights:**
- Retailer stage has the highest delay (23.59 hrs).  
- Delay trend decreases from Aug–Dec.  
- Delivery completion ≈ 52%.  

---

### 🔸 Page 2 – Risk & Disruption Analysis
**Includes:**
- KPIs: Total Disruptions (1K), Avg Delay (23.95 hrs)  
- Bar Charts: Risk Types, Risk Delays  
- Table: Top Delayed Routes  
- Cards: Top Risk (Traffic), Most Affected Stage (Retailer)  

**Insights:**
- Traffic is the most frequent risk.  
- Equipment Failure causes the longest delays.  
- Retailer stage faces the most disruptions.  

---

### 🔸 Page 3 – Cost and Efficiency Insights
**Includes:**
- KPIs: Avg Cost per Delivery ($269), Highest Cost Route (Route_621)  
- Pie Chart: Cost by Region  
- Bar Chart: Partner Costs  
- Table: Costliest Routes  
- Line Chart: Transactions per Month  

**Insights:**
- Carrier B and Supplier A are most costly.  
- Urban region contributes 86% of total cost.  
- Warehouse stage has most successful deliveries (56%).  

---

### 🔸 Page 4 – Environmental & GPS Tracking
**Includes:**
- KPIs: Avg Temp (17.07°C), Humidity (50%), Speed (54.86 km/h)  
- Dual Line Chart: Temperature & Humidity over Time  
- Combo Chart: Speed vs Delay by Stage  

**Insights:**
- Manufacturing is fastest (57 km/h).  
- Retailer has lowest speed but highest delay.  
- Environmental factors have minimal effect.  

---

## 💡 Key Insights Summary

| Category | Findings |
|-----------|-----------|
| **Stage** | Logistics & Warehouse cause most delays |
| **Region** | Rural areas have higher delay & cost |
| **Route** | Few routes are consistently slow |
| **Entity** | Some entities are efficient; others face disruptions |
| **Speed** | No clear link with delay |
| **Weather** | Minor impact on performance |

---

## 🎯 Business Impact
This analysis helps businesses pinpoint where time and money are being lost.

By improving the Logistics and Warehouse stages and optimizing underperforming routes, organizations can:
- Reduce delivery delays  
- Cut logistics costs  
- Improve coordination  
- Make data-driven decisions  

---

## ✨ Final Conclusion
This project demonstrates how **data analysis and visualization** reveal deep insights into supply chain efficiency.

Using **Python for EDA** and **Power BI for dashboards**, raw data was turned into actionable insights.

**Key takeaway:**  
Delays are mainly caused by **Logistics inefficiency and regional challenges**, not speed or weather.  
Targeting these areas can greatly improve delivery time and cost performance.
