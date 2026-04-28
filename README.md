# real-estate-market-analysis
Analyze property listings, sales trends, and market dynamics in a real estate database

Real Estate Market Analysis - SQL Project

📌 Project Overview

This repository contains SQL queries and analysis scripts for a real estate market intelligence project for MetroCity brokerage. The project analyzes property listings, sales transactions, agent performance, and neighborhood trends to deliver data-driven insights for investment, pricing, and operational strategies.

 

🎯 Business Objectives

As a data analyst, the goal is to answer critical business questions:

- How do sale prices compare to listing prices across neighborhoods?
​
- How does property size impact pricing trends by property type and location?
​
- Which agents drive the highest sales volume and commission efficiency?
​
- Do property inspections and identified issues influence final sale prices?
​
- Which neighborhoods offer the strongest long-term investment potential?

 

🗄️ Database Schema

The database  real_estate  consists of 5 core tables with the following structure:
 
TABLE -

       properties - id ,  address ,  neighborhood_id ,  property_type ,  bedrooms , bathrooms ,  sqft ,  list_price ,  list_date -  Stores property details,                                                                                                                   specifications, and initial listing information 

       Sales -  id ,  property_id ,  agent_id ,  sale_price, Tracks transaction records, including pricing and time to sell
       
       agents - id ,  name ,  experience_years ,  specialization ,  commission_rate - Contains agent profiles, expertise, and compensation structure 
       
       neighborhoods - id ,  name ,  city ,  avg_income ,  school_rating , walkability_score - Provides demographic and livability metrics for each area
       
       inspections - id ,  property_id ,  inspection_date ,  issues_found , severity_score - Records inspection results and quality issues identified before sale

       
🚀 Analysis Challenges

The project is structured into 5 core analytical challenges:

1. Price-to-List Ratio Analysis

Calculate the ratio of final sale price to original listing price, aggregated by neighborhood. Identifies pricing flexibility, market demand, and negotiation trends.

2. Property Size vs Price Analysis

Analyze price per square foot trends across property types and neighborhoods. Uncovers how size, location, and property category influence valuation.

3. Agent Performance & Commission Analysis

Evaluate agents based on sales volume, average days on market, total commission earned, and performance efficiency. Helps identify top performers and training opportunities.

4. Inspection Impact on Sale Price

Measure how the number/severity of property issues affects final sale prices. Quantifies the financial impact of property condition and repair needs.

5. Neighborhood Investment Score

Build a composite scoring system combining income levels, school quality, walkability, and price trends to rank neighborhoods by investment potential.

 

🛠️ Skills Demonstrated

- Complex SQL querying (JOINs, aggregations, window functions)
​
- Data normalization & schema understanding
​
- Metric calculation & KPI development
​
- Business logic implementation
​
- Data-driven reporting & insight generation

 

📂 Repository Structure
real-estate-sql-analysis/
├── queries/

│   ├── 01_price_to_list_ratio.sql

│   ├── 02_size_vs_price_analysis.sql

│   ├── 03_agent_performance.sql

│   ├── 04_inspection_impact.sql

│   └── 05_investment_scoring.sql

├── schema/

│   └── create_tables.sql          # Database creation script

├── reports/

│   └── analysis_summary.md        # Key findings & insights

└── README.md
 

 

▶️ How to Use

1. Run  schema/create_tables.sql  to set up the database and tables.
​
2. Execute individual query files from the  queries/  folder to generate insights.
​
3. Modify parameters or add custom filters to adapt analysis to specific cities or time periods.

 

📊 Example Outputs

- Neighborhood-wise price-to-list ratios showing premium/discount trends
​
- Price per sqft heatmaps by property type
​
- Agent leaderboards based on sales efficiency
​
- Correlation analysis between inspection severity and price reductions
​
- Investment score rankings for targeted property acquisitions
