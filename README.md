# Finance-KPI-Dashboard

## Finance KPI Dashboard – Executive Financial Performance Analysis

### About the Project
This project involves building a high-impact Finance KPI Dashboard in Power BI designed to track team sales performance against set targets. The analysis covers 14 months of data, from January 2023 through February 2024. The dashboard provides both a high-level summary of critical financial metrics and a detailed view of individual salesperson performance.
### Built With

•	Power BI Desktop: For data modeling and visualization.

•	Power Query: For data cleaning, unpivoting, and transformation.

•	DAX (Data Analysis Expressions): For calculating complex KPIs and dynamic titles.

### Data Preparation
The project utilizes four primary data tables:

1.	Actual Performance: Monthly sales performance by salesperson.   
2.	Targets: Monthly sales targets for each salesperson.   
3.	Calendar Dimension: Monthly dates, enhanced with "Year" and "Month Name" columns for easier analysis.   
4.	People Dimension: Metadata regarding the sales team.
   
### Key ETL Steps:

•	Unpivoting: Transformed "Matrix" style reports into a standard three-column table (Salesperson, Month, Sales) to facilitate analysis.

•	Data Typing: Fixed date and numerical data types to ensure calculation accuracy.

### Data Modeling
The data model follows a tidy schema with two fact tables—Actuals and Targets—positioned at the center, connected to the Calendar and People dimension tables. Relationships were established using the date and salesperson columns to ensure seamless filtering across all visuals.

### DAX Measures
Several key measures were developed to drive the dashboard's insights:

•	Core KPIs: Total Sales Actual, Total Sales Target, Variance, and Variance %.

•	Time Intelligence: Year-to-Date (YTD) calculations for sales, targets, and variance using the DATESYTD function.

•	Performance Indicators:

    o	Target Reached Month Count: Counts the number of months where the target was met.

    o	Dynamic Visual Labels: A custom measure using Emoji symbols (green and red circles) to visually represent positive or        negative variance.

    o	Dynamic Title: A measure that automatically updates the chart title to show performance status (e.g., "We met targets        for 2 out of 14 months").

### Dashboard Features
•	Executive Summary Cards: Utilizes the "New Card Visual" to show main KPIs alongside YTD reference labels for 
   immediate context.

•	Win/Loss Chart: A conditional-formatted column chart indicating which months met targets (Green) or missed them (Red).

•	Actual vs. Target Trend: An overlapping column chart where the Target is shown with 50% transparency in the 
   background and Actual performance in the foreground.

•	Team Performance Table: A detailed list featuring:

    o	Employee Photos: Categorized as Image URLs.

    o	Conditional Formatting: Integrated Data Bars for actual values and variance.

    o	Sparklines: Inline trend graphs showing sales performance over time for each individual.

•	Interactive Slicers: Filters for team selection that update all visuals and dynamic narratives.

•	Smart Narrative: A dynamically generated text summary that explains current performance trends in plain language.

### Insights
Despite the visually appealing interface, the data reveals a challenging period where the team met targets in only 2 out of 14 months. The dashboard allows stakeholders to drill down into specific months or individual team members to identify root causes of underperformance.

### 7. Screenshots / Demos
The dashboard looks like.

Example:![Dashboard Preview](https://github.com/sithara-sreedharan/Finance-KPI-Dashboard/blob/main/Snapshot%20of%20Finance%20KPI%20Dashboard.png)
