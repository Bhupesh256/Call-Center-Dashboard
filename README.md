# 📞 Call Center Performance Dashboard in Excel

An interactive and visually dynamic Excel dashboard project built to analyze call center performance using **Power Pivot**, **DAX**, **PivotTables**, **Slicers**, and **Conditional Formatting**.

## 🧠 Project Overview

This project demonstrates how to build a **Call Center Performance Dashboard** in Microsoft Excel, showcasing the following core data analytics capabilities:

- Data modeling using **Power Pivot**
- Calculated metrics using **DAX (Data Analysis Expressions)**
- Interactive filtering with **Slicers**
- Trend analysis using **PivotCharts**
- Real-time performance tracking of customer service representatives
- Advanced **conditional formatting** for better visual storytelling

---

## 🎯 Key Objectives

- Analyze call center activities and customer satisfaction
- Monitor performance of individual representatives
- Enable management to make data-driven decisions
- Create an interactive dashboard with drill-down insights

## 📊 Key Performance Indicators (KPIs)

| KPI Metric                        | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| Total Calls                      | Total number of calls handled by all reps                                  |
| Purchase Amount (Sum)            | Total value of purchases resulting from calls                              |
| Average Satisfaction Rating      | Average customer feedback rating (1–5 scale)                               |
| 5-Star Ratings Count             | Number of calls receiving a perfect satisfaction score                     |
| Calls by Day of the Week         | Distribution of call volumes across weekdays                               |
| Calls Over Time                  | Time series trend of total calls by day/month                              |
| Representative Performance       | Metrics for individual agents: call count, satisfaction, purchase value    |

## 📌 Dataset Overview

### `calls_data.xlsx`
- Call Number
- Customer ID
- Representative Name
- Date of Call
- Purchase Amount
- Satisfaction Rating
- Derived fields (weekday, call hour, etc.)

### `customer_data.xlsx`
- Customer ID
- Gender
- Age
- City

---

## ⚙️ Features & Tools Used

| Excel Feature         | Purpose                                                                 |
|----------------------|-------------------------------------------------------------------------|
| Power Pivot           | Combine multiple tables and create relationships                       |
| PivotTables & Charts | Summarize and visualize KPIs                                            |
| DAX Measures          | Calculate custom KPIs (e.g., total calls, average ratings)             |
| Slicers               | Filter by representative, date, city, etc.                             |
| Trend Charts          | Show volume over time and across days                                  |
| Conditional Formatting| Highlight selected representatives and KPIs                            |
| Form Controls & Shapes| Design professional and responsive dashboard layout                    |

---

## 🛠️ Implementation Steps

### 1. **Data Review & Setup**
- Load and clean call and customer data
- Designate a consistent theme and color scheme
- Prepare icons and images for use in visual layer

### 2. **Modeling & Relationships**
- Add datasets to **Excel Data Model**
- Link `CustomerID` between `Calls` and `Customers` tables

### 3. **Create Measures Using DAX**
- `Total Calls = COUNTROWS(Calls)`
- `Total Purchase = SUM(Calls[Purchase Amount])`
- `Average Rating = AVERAGE(Calls[Satisfaction Rating])`
- `Five Star Ratings = CALCULATE(COUNTROWS(Calls), Calls[Satisfaction Rating] = 5)`

### 4. **Pivot Tables for Metrics**
- Create base pivot tables for KPIs
- Link slicers for representative and city filtering

### 5. **Build the Dashboard Layout**
- Use shapes, text boxes, and charts to design layout
- Link pivot values to cells for dynamic updates
- Apply conditional formatting to highlight reps or trends

### 6. **Trend Graphs & Visualizations**
- Line/column charts for call trends over time
- Dual-axis charts for comparing calls vs. revenue
- Day-of-week analysis to highlight call patterns

### 7. **Add Representative Insights**
- Insert rep photos and link them to slicer selections
- Display dynamic rep performance using formulas
- Highlight top performers using conditional logic

---

## 📈 Project Insights

- 🚀 **Representative Comparison**: Visual side-by-side performance evaluation
- ⭐ **Customer Satisfaction Trends**: Identifying agents with highest 5-star ratings
- ⏳ **Peak Time Analysis**: Call volumes by day/time reveal operational bottlenecks
- 📉 **Revenue Attribution**: See which reps contribute most to purchases
- 🧠 **Actionable Design**: Fully interactive dashboard helps make real-time decisions

---


## 📷 Screenshots

<img width="1740" height="803" alt="Screenshot 2025-08-06 100447" src="https://github.com/user-attachments/assets/6bb7ef78-3f6a-4654-a2bd-91eef0e8f565" />

---

## 🧪 How to Use

1. Clone this repo:
   ```bash
     https://github.com/Bhupesh256/Call-Center-Dashboard
   ```
2. Open `Call Center Dashboard.xlsx`
3. Use slicers to explore rep-specific or time-based performance
4. Modify datasets or add new reps to update insights automatically
