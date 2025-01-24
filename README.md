# [Project 1: Data Warehousing for Aircall data]
 
# Project Overview
The Patient Advisory Team (PAT) at the company advises patients on healthcare products and services through phone calls facilitated by **Aircall**, a cloud-based telephony platform. The board tasked me with building a **data warehouse** to centralize, organize, and analyze PAT performance data. The data warehouse provides insights into key metrics such as call duration, advisor availability, and patient engagement, enabling management to evaluate team performance and operational efficiency.
 
# Objectives
- **Data Centralization**: Integrate raw data from the Aircall API into a structured data warehouse for analysis.
- **Data Modeling**: Design a scalable schema to store and query key metrics, including:
  - Call Logs
  - Advisor Availability
  - Patient Interaction and Engagement
- **Performance Monitoring**: Enable analysis of team effectiveness using metrics such as:
  - Total Calls
  - Average Call Duration
  - Advisor Utilization Rates
  - Message Delivery Metrics
- **Visualization**: Provide actionable insights through interactive Tableau dashboards tailored for non-technical stakeholders.
 
# Project Workflow
- **Data Integration**:
  - Connected to the Aircall API to extract datasets such as call logs, availability, and engagement data.
  - Automated data ingestion pipelines to retrieve and store the data into MariaDB.
 
- **Data Warehouse Design**:
  - Designed a **star schema** with fact and dimension tables to facilitate efficient querying and reporting:
    - Fact Table: Call logs with metrics like duration and engagement.
    - Dimension Tables: Advisors, time, and interaction categories.
  - Normalized data to reduce redundancy and ensure scalability.
 
- **ETL Pipeline Development**:
  - Built an ETL (Extract, Transform, Load) process to:
    - Extract raw data from the Aircall API.
    - Transform data to align with the data warehouse schema.
    - Load processed data into MariaDB tables.
 
- **Data Analysis**:
  - Queried the data warehouse to calculate performance metrics:
    - Total calls made by each advisor.
    - Average call duration and time of day trends.
    - Advisor availability and utilization rates.
    - Patient interaction metrics like message success rates.
 
- **Dashboard Creation**:
  - Designed a Tableau dashboard to visualize:
    - Team and individual performance.
    - Trends in call activity and advisor availability.
    - Metrics for patient engagement and outcomes.
 
# Challenges and Solutions
**API Data Integration**
- **Challenge**: Complex, nested data structures from the Aircall API.
- **Solution**: Flattened data structures during the ETL process to fit the data warehouse schema.
 
**Schema Design**
- **Challenge**: Balancing schema flexibility with query performance.
- **Solution**: Implemented a star schema to support both complex analysis and scalability.
 
**Data Quality**
- **Challenge**: Inconsistent and missing data from the source.
- **Solution**: Added validation checks and transformations in the ETL pipeline to ensure data integrity.
 
**Stakeholder Reporting**
- **Challenge**: Presenting technical insights in a non-technical format.
- **Solution**: Created simplified Tableau dashboards with clear visualizations and tooltips for contextual understanding.
 
# Technologies Used
- **Data Integration**:
  - Aircall API for data extraction.
- **Data Warehouse**:
  - MariaDB for schema design and data storage.
- **ETL Pipeline**:
  - SQL for data transformation and loading.
  - Python (for automation scripts).
- **Data Visualization**:
  - Tableau for interactive dashboards.
 
# Outcome
- **Centralized Data Warehouse**: Built a robust data warehouse to store and manage PAT performance data.
- **Actionable Insights**: Enabled management to track advisor performance, operational efficiency, and patient engagement.
- **Scalable Solution**: Designed a schema capable of handling growing data volumes and new performance metrics.
