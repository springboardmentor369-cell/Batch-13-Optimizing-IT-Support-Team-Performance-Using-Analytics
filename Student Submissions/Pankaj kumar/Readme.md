📊 IT Support Team Performance Dashboard
📌 Problem Statement

Customer support teams handle thousands of tickets related to product issues, service requests, and technical problems. Efficient management and analysis of these tickets are essential to improve customer satisfaction and service quality.

This project aims to analyze customer support ticket data and build an interactive dashboard to understand ticket patterns, response times, customer satisfaction, and support channel performance.

📁 Dataset Description

The dataset contains customer support ticket records, including customer details, product information, ticket attributes, and resolution metrics.

📌 Dataset Features
Ticket ID – Unique identifier for each support ticket
Customer Name – Name of the customer
Customer Email – Email of the customer
Customer Age – Age of the customer
Customer Gender – Gender of the customer
Product Purchased – Product bought by the customer
Date of Purchase – Date when the product was purchased
Ticket Type – Type of issue raised
Ticket Subject – Subject of the support ticket
Ticket Description – Detailed description of the issue
Ticket Status – Status of the ticket (Open, Closed, Pending)
Resolution – Resolution provided by the support team
Ticket Priority – Priority level (High, Medium, Low)
Ticket Channel – Channel used (Email, Phone, Chat, Social Media)
First Response Time – Time taken for the first response
Time to Resolution – Time taken to resolve the issue
Customer Satisfaction Rating – Rating given by the customer

📊 Total Records: 8469

🔍 Exploratory Data Analysis (EDA)

The following preprocessing steps were performed:

Data cleaning and handling missing values
Removal of null and inconsistent records
Data transformation using Power Query
Validation of time-related fields
Aggregation and grouping for analysis
📈 Key Insights
The system handles a high volume of tickets (5650 tickets analyzed in dashboard view).
Nearly half of the tickets are resolved, indicating scope for improving efficiency.
All support channels (Email, Phone, Chat, Social Media) are used almost equally.
Certain products (e.g., Sony Xperia, iPhone) generate more support tickets.
Customer satisfaction is moderate, with most ratings in the mid-range.
Some channels show a higher proportion of pending tickets, indicating delays.
No strong direct correlation is observed between resolution time and satisfaction.
💡 Recommendations

Based on the analysis:

Improve product quality for frequently reported products
Allocate more resources to high-volume channels
Prioritize high-priority tickets for faster resolution
Optimize workflows to reduce response and resolution time
Implement automation for handling common issues
🛠 Tools & Technologies Used
Power BI → Dashboard creation and visualization
Microsoft Excel → Data preprocessing
Power Query → Data transformation
GitHub → Version control and documentation
