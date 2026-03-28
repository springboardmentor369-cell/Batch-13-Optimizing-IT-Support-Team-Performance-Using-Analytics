# 📊 IT Support Ticket Operations Dashboard (Power BI)

## 🔹 Project Overview

This project presents an interactive **IT Support Dashboard** developed using Power BI to analyze and monitor ticket operations. The dashboard provides insights into ticket volume, resolution efficiency, SLA compliance, and support agent performance.

The goal of this project is to transform raw ticket data into meaningful insights that help improve decision-making and operational efficiency in IT support services.

---

## 🎯 Objectives

* Monitor total ticket workload and status distribution
* Analyze ticket trends over time
* Evaluate SLA compliance and breaches
* Measure resolution and response efficiency
* Track support agent performance
* Identify bottlenecks in IT support operations

---

## 📁 Dataset Description

The dataset consists of IT support ticket records with the following fields:

* Ticket ID
* Date
* Status (Open, Closed, In Progress)
* Priority (High, Medium, Low)
* Category (Network, Software, Hardware, etc.)
* Support Agent
* Resolution Time (hours)
* First Response Time (hours)
* SLA Limit (hours)

---

## 🧹 Data Cleaning (Power Query)

The dataset was cleaned and transformed using Power Query:

* Removed duplicates and unnecessary columns
* Handled missing/null values
* Standardized date formats
* Converted data types (text, date, numeric)
* Trimmed and cleaned text fields

---

## 📊 Key KPIs

The dashboard includes the following Key Performance Indicators:

* Total Tickets
* Open Tickets
* Closed Tickets
* Pending Tickets
* Average Resolution Time
* SLA Compliance (%)
* SLA Breach Count

---

## 📈 Dashboard Features

### 1. Ticket Status Distribution

* Donut chart showing Open, Closed, and In Progress tickets

### 2. Ticket Trends Over Time

* Line chart to analyze ticket volume across dates

### 3. Tickets by Priority

* Bar chart displaying High, Medium, and Low priority tickets

### 4. Tickets by Category

* Stacked chart showing issue types and their status

### 5. Resolution Time Analysis

* Average resolution time by category

### 6. SLA Performance

* Gauge visual showing SLA compliance percentage

### 7. Agent Performance

* Charts and table showing:

  * Tickets handled
  * Resolution time
  * First response time

### 8. Interactive Filters (Slicers)

* Date
* Priority
* Category
* Support Agent

---

## 🧮 Key Calculations (DAX)

```DAX
Total Tickets = COUNT(Tickets[Ticket ID])

Open Tickets = CALCULATE(COUNT(Tickets[Ticket ID]), Tickets[Status] = "Open")

Closed Tickets = CALCULATE(COUNT(Tickets[Ticket ID]), Tickets[Status] = "Closed")

SLA Compliance % =
DIVIDE(
    CALCULATE(COUNT(Tickets[Ticket ID]), Tickets[SLA Met] = "Yes"),
    COUNT(Tickets[Ticket ID])
) * 100
```

---

## 📌 Key Insights

* Majority of tickets are successfully closed within SLA
* High priority tickets require faster resolution
* Certain categories (e.g., hardware/security) have higher resolution times
* Agent performance varies based on workload and efficiency

---

## 🚀 Tools & Technologies Used

* Power BI (Dashboard & Visualization)
* Power Query (Data Cleaning)
* DAX (Calculations & Measures)
* Microsoft Excel (Dataset)

---

## 📊 Business Impact

This dashboard helps:

* Improve IT service efficiency
* Monitor SLA performance
* Optimize resource allocation
* Enhance customer satisfaction

---

## 🔮 Future Improvements

* Add predictive analytics for ticket trends
* Include ticket aging analysis
* Integrate real-time data sources
* Add customer satisfaction metrics

---

## 👨‍💻 Author

Pradeep Kumar
B.E. CSE Student, Chandigarh University

---

## 📌 Conclusion

This project demonstrates how data visualization and analytics can be used to improve IT support operations by providing actionable insights and performance monitoring.

