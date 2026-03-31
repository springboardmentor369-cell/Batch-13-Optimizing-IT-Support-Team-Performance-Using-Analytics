# README – IT SUPPORT TEAM PERFORMANCE ANALYSIS USING POWER BI
---

# 📌 Project Title

**Optimizing IT Support Team Performance using Data Visualization (Power BI)**

---

# 📖 Project Overview

This project focuses on analyzing IT support call center ticket data to evaluate the performance of a technical support team and identify areas for improvement. The dataset consists of various attributes such as Ticket ID, Call Date, Resolution Date, Agent Name, Department, Issue Type, Priority, Status, Channel, Region, Handle Time, Wait Time, First Call Resolution, SLA Met, Satisfaction Score, OS Type, Shift, Escalated, Reopen Count, Cost Per Ticket, and Agent Experience.

The primary aim of this project is to convert raw and unstructured call center data into meaningful insights using Power BI. The entire workflow includes data cleaning, transformation, exploratory data analysis (EDA), data modelling, DAX calculations, and dashboard creation.

By implementing a structured analytical approach, the project enables better decision-making and performance optimization for IT support call center operations.

---

# 🎯 Objectives

* To understand and analyze IT support call center ticket data
* To identify performance gaps in the support team
* To measure key performance indicators (KPIs) such as SLA compliance and First Call Resolution
* To build interactive dashboards for decision-making
* To apply Power BI concepts such as DAX, data modelling, and visualization
* To evaluate agent performance across shifts, regions, and channels

---

# 🔄 Project Workflow (Detailed Week-wise Execution)

---

## 🔹 Week 1 – Problem Analysis and Dataset Understanding

In the initial stage, the problem statement was clearly defined. The objective was to optimize IT support call center team performance by analyzing ticket and call data.The dataset (1,030 raw records × 22 columns) was explored in detail. Important columns were identified including Ticket_ID, Call_Date, Call_Time, Resolution_Date, Agent_Name, Department, Issue_Type, Priority, Status, Channel, Region, Handle_Time_Minutes, Wait_Time_Seconds, First_Call_Resolution, SLA_Met, Satisfaction_Score, OS_Type, Shift, Escalated, Reopen_Count, Cost_Per_Ticket_USD, and Agent_Experience_Yrs.



Data types were verified and initial observations were made regarding missing values (up to 280 in some columns), duplicate entries (30 records), and inconsistent formatting across categorical fields. This stage helped define the scope of analysis.

---

## 🔹 Week 2 – Power BI Practical Working

In this week, the Power BI environment was explored. The interface components such as Ribbon, Canvas, and Visualization Pane were studied.

Different views in Power BI were analyzed:

* Report View for creating dashboards
* Data View for inspecting data
* Model View for managing relationships

Power Query Editor was introduced as a tool for data transformation. Basic operations such as loading data, filtering rows, and modifying columns were performed.

---

## 🔹 Week 3 – Data Cleaning (Team-Based Approach)

Data cleaning was performed using Power Query Editor to prepare the dataset for analysis. The raw dataset contained 1,030 records with significant quality issues across all 22 columns.

The following cleaning steps were implemented:


* Removal of duplicate records using Ticket ID
* Deletion of irrelevant columns to reduce complexity
* Handling missing values by either removing or replacing them
* Standardizing inconsistent values (e.g., "high" → "High")
* Converting data types (text to date/time)
* Creating new columns such as Resolution Time and Ticket Age

This stage ensured that the dataset became clean, consistent, and analysis-ready.

---

## 🔹 Week 4 – KPI Cards and Performance Metrics

Key Performance Indicators (KPIs) were identified to measure support team performance. KPI cards were created in Power BI to display important metrics such as:

* Total number of tickets handled
* Average handle time (minutes)
* Average wait time (seconds)
* SLA compliance percentage
* First Call Resolution (FCR) rate
* Average customer satisfaction score
* Escalation rate
* Average cost per ticket (USD)

Additionally, key business questions were framed to guide dashboard development:

1. Distribution of tickets by priority level and issue type
2. Average resolution and handle time by agent and department
3. Top-performing support agents by satisfaction score and FCR
4. Regional distribution and volume of tickets
5. SLA compliance and escalation trends over time
6. Channel-wise and shift-wise performance comparison

These metrics and questions formed the foundation for visualization.

---

## 🔹 Week 5 – Exploratory Data Analysis (EDA)

EDA was performed to understand patterns and trends in the dataset. Power BI features such as Column Distribution, Column Profile, and Column Quality were used in Power Query Editor.

Key activities included:

* Analyzing ticket volume distribution across Priority, Status, Channel, and Shift
* Profiling Handle_Time_Minutes and Wait_Time_Seconds distributions
* Identifying patterns in SLA breaches by region and department
* Detecting agents with consistently low satisfaction scores
* Analyzing reopen count and escalation patterns
* Understanding OS_Type distribution for targeted support

Visualizations such as bar charts, line charts, and histograms were used to explore the data. Outliers in Satisfaction_Score (−1, 99) and Handle_Time_Minutes (negative values) were identified and handled during cleaning. This stage improved understanding of the dataset and supported better decision-making.

---

## 🔹 Week 6 – Data Modelling and Live Data Import

Data modelling was implemented using the Star Schema approach. The cleaned call center dataset was treated as the Fact Table, and separate Dimension Tables were created.

Key concepts applied:

* Fact Table containing measurable values (handle time, wait time, cost, satisfaction score)
* Dimension Tables for Agent, Department, Region, Channel, Issue Type, OS Type, and Shift
* Primary Key and Foreign Key relationships (e.g., Ticket_ID, Agent_Name)
* Cardinality types: 1:1, 1:Many, Many:1
* One-to-Many relationships for efficient cross-filtering in dashboards

Live data import was explored using APIs. The following restrictions were observed:

* URLs without authentication cannot be accessed
* API rate limits restrict frequent data requests
* Dynamic web content cannot be loaded directly
* Data privacy settings may block external connections

This week I ensured a strong data structure and improved dashboard performance.

---

## 🔹 Week 7 – DAX, Measures, Visuals and Dashboard Creation

In this week , DAX was used to create measures for advanced calculations. Both implicit and explicit measures were implemented.

* Implicit measures were automatically generated by Power BI for quick summaries
* Explicit measures were created using DAX formulas for precise KPI calculations

Key DAX measures developed:

* Total Tickets = COUNT(Ticket_ID)
* FCR Rate = DIVIDE(COUNTIF(First_Call_Resolution, "Yes"), Total Tickets)
* SLA Compliance % = DIVIDE(COUNTIF(SLA_Met, "Yes"), Total Tickets)
* Avg Satisfaction = AVERAGE(Satisfaction_Score)
* Avg Handle Time = AVERAGE(Handle_Time_Minutes)
* Escalation Rate = DIVIDE(COUNTIF(Escalated, "Yes"), Total Tickets)

Visualizations were created using bar charts for comparison, pie charts for distribution, line charts for trends, and cards for KPI display. Slicers were added to enable interactive filtering based on Priority, Department, Region, Channel, and Shift.

Three dashboards were created:

### 1. IT Support Ticket Overview Dashboard

Provides summary KPI cards (total tickets, avg handle time, SLA %, FCR rate), ticket distribution by priority, status, issue type, and channel. Includes time-series trends for ticket volume.

### 2. Support Team Performance Dashboard

Analyzes individual agent performance including satisfaction score, handle time, SLA compliance, escalation rate, and FCR. Includes shift-wise and department-wise performance breakdowns.

### 3. Ticket Analysis and Insights Dashboard

Explores regional ticket distribution, OS type trends, reopen count analysis, cost per ticket breakdown, and wait time patterns by channel and region.

Each dashboard followed a structured layout with KPI cards at the top, charts in the middle, and detailed analysis at the bottom.

---

# 📊 Dashboard Design Approach

The dashboards were designed with a focus on clarity, usability, and interactivity.

* KPI cards placed at the top for quick insights
* Charts arranged logically for better understanding
* Slicers added for dynamic filtering by Priority, Department, Region, Channel, and Shift
* Consistent color themes applied throughout all dashboards
* Proper alignment and spacing maintained

This structured design improves user experience and supports effective decision-making.

---

# 🛠️ Tools and Technologies Used

* Power BI Desktop
* Power Query Editor
* DAX (Data Analysis Expressions)
* Python (pandas, openpyxl) for initial data cleaning
* Excel / CSV dataset (Raw: 1,030 rows | Cleaned: 1,000 rows | 22 columns)

---

# 🔍 Key Concepts Implemented

* Data Cleaning and Transformation (22 documented cleaning steps)
* Exploratory Data Analysis (EDA)
* Data Modelling (Star Schema)
* Cardinality Relationships (1:1, 1:Many)
* DAX Measures (Base and Composite)
* Dashboard Design and Visualization
* Live Data Integration (API exploration)

---

# ⚠️ Challenges Faced

* Handling missing values across multiple columns (up to 280 missing in Satisfaction_Score)
* Standardizing 6+ date formats across Call_Date and Resolution_Date
* Fixing typos and casing inconsistencies in Priority and Issue_Type fields
* Identifying correct data model relationships without a pre-defined schema
* Managing out-of-range values in numeric fields
* Handling API and URL restrictions during live data exploration
* Designing clear and user-friendly dashboards for a multi-column dataset

---

# ✅ Outcomes

* Clean and structured dataset (1,000 rows, zero nulls, zero duplicates)
* Efficient star schema data model with proper relationships
* Interactive dashboards with slicers for dynamic filtering
* Accurate KPI metrics: FCR rate, SLA compliance, satisfaction scores
* Meaningful insights into agent performance, regional trends, and cost analysis
* Reusable Power Query M code and DAX measures

---

# 📌 Conclusion

This project demonstrates the effective use of Power BI for analyzing IT support call center data and improving team performance. By following a structured approach from data understanding to dashboard creation, the project successfully converts raw, inconsistent data into actionable insights.

It highlights the importance of data preparation, modelling, and visualization in real-world data analysis scenarios, particularly for IT support operations where SLA compliance, agent efficiency, and customer satisfaction are critical KPIs.

---

# 🚀 Future Scope

* Integration with real-time databases and ticketing systems 
* Advanced DAX and time intelligence functions for trend forecasting
* Predictive analytics using machine learning for ticket escalation prediction
* Deployment using Power BI Service for sharing dashboards across teams
* Row-Level Security (RLS) for department-specific access control


