#  Traffic & Acquisition Analytics – E-Commerce Project (Power BI)

# Overview
I have Analyzed e-commerce traffic sources using Google Analytics-style data. Created DAX measures for conversion rate, AOV, and channel-wise performance. Identified high-ROI marketing channels and user drop-off points. Built interactive Power BI dashboards to track sessions, revenue, conversion rate, and bounce rate. Delivered actionable insights to optimize marketing spend and improve conversions.

# Project Objective (Business View)
The goal of this project is to understand where users come from, how they behave, and which traffic sources generate revenue so marketing teams can optimize spend and conversions. 

# Dataset
I have used Google-Analytics style e-commerce dataset which can be easily found on Kaggle. This dataset has columns as Date, User_ID, Session_ID, Source, Medium, Channel, Device, Sessions, Transactions, Revenue, Bounce.

# Key questions the project answers: 
1. Which channels bring the most traffic?
2. Which channels generate the most revenue?
3. Where are users dropping off?
4. Which source has the best conversion rate?


# Load data into Power BI
1. Open Power BI desktop
2. click Get Data - CSV/Excel file
3. Load the dataset
4. Go to Power Query Editor

# Cleaning steps ( Clean data ensures correct KPIs and DAX calculations)
1. Removed Null values
2. Converted Date to Date format
3. Renamed column for clarity
4. Ensured Sessions, Revenue, Transactions are numeric

# Data Modeling ( Proper modeling improves performance and accuracy)

Since, I have used a single table, there was not a need for data modeling.

# Core DAX measures for this projects are as mentioned

Total Sessions = SUM('Traffic'[Sessions])

Total Users = DISTINCTCOUNT('Traffic'[User_ID])

Total Revenue = SUM('Traffic'[Revenue

Total Orders = SUM('Traffic'[Orders])

Conversion Rate = DIVIDE([Total Orders], [Total Sessions])

Bounce Rate = DIVIDE(SUM('Traffic'[Bounce]), [Total Sessions])

AOV = DIVIDE([Total Revenue], [Total Orders])

# Dashboard Design

  ## KPI Cards
    1. Total Session
    2. Total Users
    3. Total Revenue
    4. Conversion Rate
    5. Bounce Rate
    
  ## Traffic Source Analysis
    Bar Chart: Sessions by Channel
    Bar Chart: Revenue by Channel
    Table: Channel | Sessions | Revenue | Conversion Rate

  ## Acquisition Funnel View
    Sessions → Orders → Revenue

  ## Device Analysis
     Sessions by Device
     Conversion Rate by Device
     Revenue by Device

  ## Time Trend
     Line chart: Sessions & Revenue by Date
     

# Business Insights














