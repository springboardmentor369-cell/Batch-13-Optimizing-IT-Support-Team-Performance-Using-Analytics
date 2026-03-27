# Infosys-Spring-Board-Internship
Infosys Spring Board IT is a 8 weeks Internship Where We Get Training and Hands on Experience On Real World Project Exposer Under The Guidance of  The Mentor -Mr Akshay Sir 
Along with We Going To Work On Our Project

Project Name: Optimizing IT Support Team Performance Using Analytics

Problem Statement - In today’s digital-driven business environment, IT support teams play a critical role in ensuring uninterrupted operations and maintaining user satisfaction. However, many organizations face challenges in effectively monitoring and optimizing IT support performance due to increasing ticket volumes, delayed response times, inefficient resource allocation, and lack of data-driven decision-making.
Traditional performance evaluation methods often rely on manual tracking or basic reporting, which fail to provide deep insights into key performance indicators such as ticket resolution time, first response time, backlog trends, technician workload distribution, and customer satisfaction levels. This lack of analytical visibility results in reduced productivity, higher operational costs, and decreased service quality.
Therefore, there is a need to develop an analytics-driven approach that leverages data visualization, performance metrics, and predictive insights to optimize IT support team efficiency. By applying data analytics techniques, organizations can identify bottlenecks, forecast workload patterns, improve resource planning, enhance service delivery, and ultimately increase customer satisfaction.
The problem addressed in this project is how to utilize analytics to measure, monitor, and improve IT support team performance in a systematic and data-driven manner. 

Data Set Description - 
Perfect — from the screenshots you shared, I can see the dataset structure clearly. Here’s a **table-format description of the columns** in your `synthetic_it_support_tickets` dataset:

| Column Name            | Description                                                                                  |
|------------------------|----------------------------------------------------------------------------------------------|
| ticket_id              | Unique identifier for each support ticket (e.g., TCKT_000001)                                |
| created_at             | Date when the ticket was created                                                             |
| customer_id            | Unique identifier for the customer raising the issue                                         |
| customer_segment       | Segment type (e.g., individual, small_business, enterprise, education)                       |
| channel                | Communication channel used (e.g., email, in_app, chat, phone_transcript)                     |
| product_area           | Product/service area related to the issue (e.g., billing, login_auth, api_integration)       |
| issue_type             | Type of issue (e.g., account_access, bug, billing_problem, security_concern, feature_request)|
| priority               | Urgency level of the ticket (e.g., low, medium, urgent)                                      |
| status                 | Current ticket status (e.g., resolved, in_progress, closed_no_action)                        |
| sla_plan               | SLA plan associated with the customer (e.g., standard, gold, platinum)                       |
| initial_message        | First message from the customer describing the issue                                         |
| agent_first_response   | First response provided by the support agent                                                 |
| agent_first_reply      | Timestamp or text of the agent’s first reply                                                 |
| resolution_summary     | Notes summarizing how the issue was resolved                                                 |
| resolution_time_hours  | Time taken to resolve the ticket (in hours)                                                  |
| reopened               | Indicator if the ticket was reopened after resolution (Yes/No)                               |
| customer_sentiment     | Sentiment expressed by the customer (e.g., positive, neutral, negative)                      |
| csat_score             | Customer satisfaction score (numeric rating)                                                 |
| has_attachment         | Whether the ticket included an attachment (Yes/No)                                           |
| platform               | Platform used by the customer (e.g., web, mobile)                                            |
| region                 | Geographic region of the customer                                                            |

 Dataset Summary
| **Attribute**      | **Details**                                            |
| ------------------ | ------------------------------------------------------ |
| Dataset Name       | Synthetic IT Support Tickets Dataset                   |
| Total Records      | 1000+ Support Tickets                                  |
| File Format        | Excel (.xls / .xlsx)                                   |
| Project Purpose    | Optimizing IT Support Team Performance Using Analytics |
| Tools for Analysis | Python, Excel, Power BI                                |


KPI - 
Average Resolution Time (hrs): 38.18
Total Tickets: 791
Reopened Tickets: 39
Average CSAT Score: 2.17
Resolved Tickets: 692

DashBoard Description - 
This dashboard provides a comprehensive overview of IT support ticket performance and customer satisfaction. It enables stakeholders to monitor operational efficiency, identify bottlenecks, and evaluate service quality across different dimensions such as:

Channels (web, app, email, chat, phone)
Issue Types (bug, feature request, performance, etc.)
Priority Levels (low, medium, high, urgent)
Customer Segments
Regions
Key Visualizations:
Donut Chart: Ticket distribution by channel
Waterfall Chart: Reopened tickets by issue type
Pie Chart: Ticket status breakdown
Line Chart: Resolution time trends by month
Bar Charts: CSAT by channel & customer segment
Tree Map: Ticket distribution by region and priority
Table: Detailed ticket-level insights

Interactive filters allow slicing data by priority, channel, and product area for deeper analysis.
Regions 

Key Insight - 
📉 Low Customer Satisfaction: Average CSAT score is 2.17, indicating poor customer experience.
⏱️ High Resolution Time: Average resolution time (~38 hours) suggests inefficiencies in handling tickets.
🔁 Reopened Tickets: 39 tickets reopened — potential quality or incomplete resolution issues.
📞 Channel Performance Variance: Some channels (e.g., chat/email) show lower CSAT compared to others.
📅 Fluctuating Resolution Trends: Monthly resolution time is inconsistent, indicating unstable workload or process gaps.
🌍 Regional Distribution: Certain regions (e.g., EU/NA) show higher ticket volumes, possibly needing more resources.
⚠️ Priority Handling: High and urgent tickets may not be resolved proportionally faster.

Recomendations -
🚀 Improve First-Time Resolution
Enhance knowledge base and agent training
Implement better diagnostic workflows
📊 Optimize High-Impact Channels
Investigate low-performing channels (e.g., chat/email)
Standardize response protocols
⏳ Reduce Resolution Time
Introduce SLA tracking dashboards
Automate repetitive tasks
🔁 Minimize Reopen Rate
Conduct root cause analysis for reopened tickets
Improve QA before ticket closure
🎯 Priority-Based Routing
Implement intelligent ticket routing for urgent/high priority issues
😊 Enhance Customer Experience
Collect detailed feedback
Introduce post-resolution follow-ups
🌐 Regional Resource Allocation
Assign more agents to high-volume regions
Adjust staffing based on demand trends

Tools Used - 
Power BI Desktop – Data visualization & dashboard creation
DAX (Data Analysis Expressions) – KPI calculations and measures
Power Query – Data cleaning and transformation
Excel / CSV Dataset – Data source (synthetic IT support dataset)
