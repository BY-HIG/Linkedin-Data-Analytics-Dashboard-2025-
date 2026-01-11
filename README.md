# Linkedin Data Analytics Dashboard (2025)

A Power BI dashboard for analyzing LinkedIn performance using DAX-driven time intelligence, calendar tables, and conditional formatting. 

![](LinkedinAnalyticsDashboard.png)

### Introduction
This project presents a LinkedIn Data Analytics Dashboard built using Power BI to analyze personal LinkedIn performance for the year 2025.
The dashboard focuses on understanding growth in connections, engagement, impressions, and posting activity, especially during the period when I became more consistent on the platform.

The goal of this project is both reflective and analytical, to review past performance, identify trends, and gain insights that can inform better content and engagement strategies going forward.

### About The Dataset
The dataset used in this project consists of personal LinkedIn activity and performance data covering the period from 2016 to 2025, with a primary focus on 2025. The data captures key metrics such as:

- Connections
- Followers
- Engagements
- Impressions
- Posts

### Data Source
- **LinkedIn Data Archive**  
  *Settings & Privacy → Data Privacy → Get a copy of your data*

- **Content Performance (Excel Export)**  
  *Profile → Analytics → Post Impressions → Export file*

### Data Preparation & Cleaning
Before building the dashboard, the raw LinkedIn data was reviewed and prepared to ensure accuracy and consistency for analysis. Key preparation steps included:

- **Data validation**: Checked date fields, numeric columns, and missing values to ensure correctness.
- **Filtering irrelevant records**: Removed rows outside the analysis scope, including incomplete or invalid date entries.
- **Date standardization**: Ensured all date fields were properly formatted to support time-based analysis.
- **Calendar table creation**: Built a custom calendar table using DAX to enable monthly trends, year-over-year comparisons, and time-intelligence calculations.
- **Handling zero and missing values**: Applied logic in measures to safely handle cases where prior-year values were zero or missing.
- **Derived metrics**: Created calculated measures for growth rates, percentage change, trends, and conditional fromatting.
- **Data modeling**: Established appropriate relationships between fact tables and the calendar table to support accurate filtering and aggregation.
- **Formatting and consistency**: Standardized number formats, percentages, and labels to improve readability and interpretation.

### Data Modelling

![](DataModel.PNG)

The data model follows a star schema design, with a central Calendar table acting as the date dimension and multiple fact tables connected to it. Core Components:

- **Calendar (Dimension Table)**
  - Acts as the central date table used for filtering and time-based analysis.
  - It contains date attributes such as Date, DateID, Month, and MonthNo, and was created using DAX.
- **Connections (Fact Table)**
  - Stores individual connection records, including connection date and related attributes.
  - Used to analyze connections growth and trends over time.
- **Followers (Fact Table)**
  - Contains daily records of new followers, linked to the calendar for trend analysis.
- **Engagement (Fact Table)**
  - Captures engagement metrics such as total engagements and impressions by date.
- **Top Posts (Fact Table)**
  - Stores post-level performance metrics, including impressions and publish dates, used to identify high-performing posts.

### KPIs Summary

- **Connections – 1,028**
  - +187.2% vs last year (549)
  - Strong signal that visibility and networking improved significantly.
  - This aligns with becoming active and visible in 2025.
- **Posts – 14**
  - +466.7% vs 3 last year
  - This explains everything else on the dashboard.
  - Posting frequency is the main driver of all other KPIs.
- **Engagements – 498**
  - “vs 0 last year” → Meaning 2024 had no meaningful engagement
  - Confirms that 2025 is the first year my content actually resonated.
- **Impressions – 14,537**
  - Also vs 0 last year
  - Shows reach expansion, even with just 14 posts.
- **Followers – 364**
  - Again vs 0 last year
  - Indicates audience building, not just vanity metrics.
 
Overall, growth was behavior-driven, not algorithm luck. Posting created visibility, visibility created engagement,  engagement created followers, and followers created more impressions.

### Chart Summary

- **Connections Monthly Trend**
  - Gradual increase across months
  - November is clearly the peak (100 connections)
  - December drops slightly
- **Followers Monthly Trend**
  - Extremely stable: mostly 30–31 followers every month
  - This is very healthy
  - No wild spikes. Indicates organic, consistent growth
- **Engagement Monthly Trend**
  - One very dominant spike in November (256 engagements)
  - Other months are relatively low but present
- **Impressions Monthly Trend**
  - Same pattern as engagement
  - November explodes (7,578 impressions)
- **Post I Made” Table**
  - Shows Post_No, Year, Month, Impressions
  - November dominates again:
    - Post-18 → 6,261 impressions
  - April, July, May also performed decently

### The Story 
After years of low activity, consistent posting in 2025 fundamentally changed my LinkedIn performance. With just 14 posts, I achieved over 1,000 new connections, 14,500 impressions, and nearly 500 engagements. Growth accelerated toward Q4, with November emerging as a breakout month for both reach and engagement. The data clearly shows that consistency, not volume, drove visibility, audience growth, and engagement.

### Skills Demonstrated
- **Excel and Power Query**
  - Data cleaning and validation
  - Handling missing and zero values
  - Data transformation
- **Power BI**
  - Data modeling and relationships
  - Interactive dashboards and reports
  - Visual and report design
- **DAX**
  - Calendar table creation
  - Time intelligence
  - Conditional formatting and KPI logic
- **Data Analysis**
  - Trend analysis
  - **Performance tracking**
  - Metric interpretation
- **Visualization & Storytelling**
  - Designing clear, insight-driven dashboards
  - Highlighting key trends and performance drivers
 
###  How to Update the Dashboard
1. Replace the LinkedIn export files with updated versions
2. Open the Power BI file
3. Refresh data

*All KPIs, trends, growth calculations, and highlights will update automatically.*
