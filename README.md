# Consumer Complaint Analysis  
**By: Taran Schlichtmann**

**Date: 11/16/2025**

SQL Analysis Using Snowflake

Focused on analyzing consumer complaints submitted to the Consumer Financial Protection Bureau (CFPB). The project required building a Snowflake database, loading complaint data, writing analytical SQL queries, and exporting results to Excel.

------------------------------------------------------------
Overview
------------------------------------------------------------

The goal of this project was to demonstrate proficiency in:

- Writing analytical SQL queries  
- Using window functions for month‑over‑month comparisons  
- Filtering and aggregating large datasets  
- Identifying trends in consumer complaints  
- Evaluating company performance based on response timeliness  
- Following SQL style guide conventions  
- Exporting reproducible results to Excel  

All work was executed in Snowflake using a custom database named **COMPLAINTS**.

------------------------------------------------------------
Repository Contents
------------------------------------------------------------

GB882_Final Project Assignment_Complaint Details_Schlichtmann_T.txt  
    All SQL statements written for the final project.

GB882_Final Project Assignment_Complaint Details_Schlichtmann_T.xlsx  
    Excel workbook containing results for all queries.

README.md  
    Documentation and context for the final project.

------------------------------------------------------------
Project Summary
------------------------------------------------------------

### Query 1 — First Complaint Received  
Identified the earliest complaint using the `date_received` field.

**Result Insight:**  
The first complaint was received on **2018‑01‑01**.

------------------------------------------------------------

### Query 2 — Most Common Financial Subproduct  
Counted complaints by **subproduct** to determine which financial product generated the most complaints.

**Result Insight:**  
The subproduct with the most complaints was **Credit reporting**.

------------------------------------------------------------

### Query 3 — Cryptocurrency Complaints in 2019  
Filtered complaints where the subproduct was **Virtual currency** and the complaint was sent to the company in **2019**.

**Result Insight:**  
The company with the most cryptocurrency‑related complaints was **Paypal Holdings, Inc**.

------------------------------------------------------------

### Query 4 — Month‑Over‑Month Complaint Changes  
Compared monthly complaint counts using `LAG()` to calculate the numeric change from the previous month.

**Result Insight:**  
Between **October 2018** and **November 2018**, complaints decreased by **2,848**.

------------------------------------------------------------

### Query 5 — Companies With Poor Timely Responses  
Calculated total complaints, untimely responses, and percent untimely responses for each company.  
Only companies with **200+ complaints** were included.

**Result Insight:**  
The company with the highest percentage of untimely responses was **Ameritech Financial**.

------------------------------------------------------------
Tools & Technologies
------------------------------------------------------------

- Snowflake (SQL execution & data exploration)  
- Excel (result storage & reporting)  
- SQL Style Guide (formatting & readability standards)

------------------------------------------------------------
Skills Demonstrated
------------------------------------------------------------

- Analytical SQL (aggregations, filtering, CASE logic)  
- Window functions (`LAG()`)  
- Date‑based analysis  
- Data quality filtering  
- Performance evaluation using calculated metrics  
- Clean, readable SQL following style conventions  
- Reproducible result export workflows  
