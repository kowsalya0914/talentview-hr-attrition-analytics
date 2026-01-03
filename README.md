# talentview-hr-attrition-analytics
Power BI workforce analytics dashboard to analyze employee attrition and retention risk.
TalentView: Workforce Risk & Retention Analytics

Project Overview
TalentView is a Power BI–based HR analytics project designed to help organizations understand employee attrition, workforce composition, and hiring effectiveness.

The project focuses on identifying attrition risk drivers, manager-level turnover patterns, and early warning signals using advanced DAX, AI visuals, and secure data modeling practices.

Business Problem
The organization is experiencing high employee turnover, but HR leadership lacks clear answers to:
  •	Why employees are leaving
  •	Which departments and managers are most affected
  •	Whether current hiring practices are effective
  •	How attrition risk is evolving over time
Without data-driven insights, retention strategies remain reactive rather than proactive.

Dataset
  •	Source: IBM HR Analytics Employee Attrition Dataset (simulated HRIS data)
  •	Records: ~1,400 employees
  •	Key Attributes:
    o	Department, Job Role, Manager
    o	Salary, Tenure, Experience
    o	Attrition Status (Voluntary / Involuntary)
    o	Demographics (Age, Gender, Education)
Personally Identifiable Information (PII) was anonymized during data preparation.

Week-Wise Project Execution

Week 1: Data Understanding, Cleaning & Anonymization
Objective
To understand the HR dataset structure and prepare it for enterprise-level workforce analysis.
Key Activities
    •	Imported raw HR data into Power BI using Power Query
    •	Assessed data quality issues (nulls, inconsistencies, duplicates)
    •	Cleaned and standardized fields (department names, job roles, dates)
    •	Anonymized sensitive employee identifiers
    •	Created derived columns for age group, tenure band, and salary band
Outcome
A clean, analysis-ready dataset suitable for workforce modeling and attrition analysis.

Week 2: Data Modeling & Core DAX Metrics
Objective
To build a scalable data model and calculate foundational workforce metrics.
Data Model
  •	Dimension Tables:
    o	Employee
    o	Department
    o	Demographics
  •	Fact Tables:
    o	Headcount (monthly snapshots)
    o	Separations (employee exits)
A star-schema-style model was used to support time-based analysis.
Core DAX Measures Created
    •	Headcount
    •	New Hires
    •	Separations
    •	Average Tenure
Outcome
Validated headcount and attrition numbers with correct filtering across departments, managers, and time.

Week 3: Advanced Metrics & Analytical Dashboards
Objective
To move from basic reporting to attrition risk analysis and hiring effectiveness.
Advanced DAX Measures
    •	Attrition Rate % (Rolling 12 Months)
    •	Voluntary vs Involuntary Attrition
    •	Time-to-Hire metrics
Dashboards Built
1. Workforce Overview
    •	KPI cards (Headcount, Avg. Tenure)
    •	Headcount by Department
    •	Demographic distribution (Gender, Age Group, Education)
2. Attrition Analysis
    •	Monthly attrition trends
    •	Separations by reason (Waterfall chart)
    •	Department- and manager-level drill-downs
AI Analysis
  •	Implemented Key Influencers visual to identify drivers of attrition
  •	Salary and Manager emerged as key contributors to voluntary exits
Outcome
Clear identification of high-risk departments and attrition drivers.

Week 4: Security, Optimization & Deployment Readiness
Objective
To align the dashboard with real-world enterprise HR analytics standards.
Row-Level Security (RLS)
    •	Managers can view only their own teams
    •	HR Business Partners can view assigned departments
    •	HR leadership has full organizational visibility
Enhancements
    •	Added slicers and bookmarks for smooth navigation
    •	Improved UI consistency and readability
    •	Optimized visuals for leadership consumption
Deployment
    •	Published to Power BI Service
    •	Configured and tested RLS roles
Outcome
A secure, multi-page HR analytics solution ready for organizational use.

Key Insights
    •	Attrition is concentrated in specific departments rather than evenly distributed
    •	Certain managers show consistently higher turnover
    •	Compensation misalignment increases early-tenure attrition
    •	Hiring speed alone does not offset retention issues

Business Recommendations
    •	Introduce manager-level retention accountability
    •	Review salary structures for high-risk roles
    •	Strengthen onboarding for early-tenure employees
    •	Monitor rolling attrition trends instead of static rates

Tools & Technologies
  •	Power BI Desktop
  •	Power Query
  •	DAX
  •	AI Key Influencers Visual
  •	Power BI Service (RLS)

