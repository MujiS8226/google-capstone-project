# Cyclistic Membership Data Analytics Case Study
This is a data analytics case study from the Google Data Analytics Certificate on Coursera, aimed at practicing data manipulation, data cleaning, data visualization, and presentation skills. As a junior data analyst, the main objective of this project is to provide compelling data insights in order to support the marketing director's strategy of maximizing profit by converting casual riders into annual members.

## Background Information
**Scenario**: You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.


**Company** **Information**: Cyclistic is a fictional bike company located in Chicago with a bike-share system of 5,824 bycicles in a network of 692 locations. Its marketing strategy previously relied on building general awareness and appealing to broad consumer segments. It offers three pricing plans: single-ride passes, full-day passes, and annual memberships, while the annual members are proved by the company financists to be more profitable to the riders buying the other two passes, referred to as casual riders.

**Business** **Objective**: Design a new marketing strategy aimed at maximizing the number of annual membership by converting casual riders into annual members, backed up with compelling data insights and professional data visualizations.

**Data Source**: The public Cyclistic trip data of previous 12 months from 04/2022 to 04/2023 provided by Google.

## Problem
The progress of this case study follows the six stages of data analysis process: ask, prepare, process, analyze, share, act. Each phase is elaborated as follows:

### Ask
- Ask data-driven questions that tackle the key objective of this capstone project and show the direction of the business analysis.
- How do annual members and casual riders use Cyclistic bikes differently?
- What are the factors that convince riders into buying the annual membership?
- How can Cyclistic use digital media to influence casual riders to become members?
### Prepare
- Understand the data structure and organize the datasets, including the data types and formats
- Keep the naming convention of the public Cyclistic trip data consistent
- Verify that the datasets follows the ROCCC method - reliable, original, comprehensive, current, cited
- Tools used for analysis:
  - Microsoft Excel: used for data cleaning and organizing the dataset
  - BigQuery: used for joining the datasets, detecting any dirty data, and analyzing the datasets
  - Tableau: used for identifying insights, creating data visualizations and a dashboard for report
- Data Directory:
  - ride_id: 16-digit ID of each ride
  - rideable_type: classic/electric/docked bike
  - started_at: starting time (date HH:MM:SS)
  - ended_at: end time (date HH:MM:SS)
  - member_casual: casual rider/annual member
  - ride_length: total length of time of each ride in minutes
  - day_of_week: day of the ride (1 Sun -7 Sat)
### Process
- Clean and manage data to help better have access to the business objective
- Remove duplicate values, missing values, biased values, fields unrelated to the business analysis
- Add additional columns to each dataset to better analyze the data
- Use Excel pivot table to categorize and summarize target data
- Data Cleaning:
    - Remove duplicate values and missing values in the datasets
    - Remove unnecessary columns: start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat, end_lng
    - Remove unrealistic values that have a ride length less than or equal to zero
    - Decide to not remove rows with too long of a ride length since it is logical for riders to forget to hand back the bike
- Creating new columns:
    - is_weekend: Yes if the day is Sunday or Saturday, No if the day is weekday
    - is_PM: True if the starting time is in PM (12:00-11:59 p.m.), False if the starting time is in AM (0:00-11:59 a.m.)
### Analyze
- Interpret the datasets and discover valuable insights related to the objective
- Calculate data for:
    - Total rides by membership
    - Average ride length by membership
    - Sum of ride length by membership
    - Maximum ride length by membership
    - The most frequent ride length by membership
    - Total rides by day of week by membership
    - Total rides by rideable type by membership
    - Average ride length by rideable type by membership
    - Total rides by hour in a day by membership
    - Average ride length by hour in a day by membership
    - Total rides by month by membership
    - Average ride length by month by membership
- Summary of data:
  - Membership: Annual members consist of 59.7% of the total riders with a total amount of 3,447,818.
  - Bike type: Among the three bike types, electric bike is the most popular by both types of riders, while classic bike is more favorable in the annual members.
   - There has been no annual members used the docked bike type in the previous 12 months, possibly due to a change in contracts.
  - Day of week: Saturday is the most popular day of the week to ride a bike, while Monday is the least popular. Annual members are more active in weekdays, with the casual riders are more active in weekends.
  - Daytime: Evening (6 p.m. - 8 p.m.) is the busiest time in a day, but morning has both the maximum and the minimum of average ride length. The average ride length by hour of members are smoother than the casual riders.
  - Month: 2022 Summer, especially June and July, are the months when the ride lengths are the longest, while the winter of 2022 has a downfall in total rides.
### Share
- Utilize visualizations and dashboard to showcase the key findings
- Use Tableau to analyze the data results and create a dashboard https://public.tableau.com/views/GooGLeDACASESTUDY/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link
### Act
- Perform business analysis to meet the interest of the stakeholders
- Post the case study online summarizing my findings

## Solutions
Recommendations based on the key insights:
- Promote annual membership using advertisements and emphasize the benefits of membership
- Provide benefits in the membership depending on preferences of the casual riders, including discounts during weekends, summers, and evenings, and for long rides
- Establish policies for not handing back the bicycles over a specific period (i.e. a week) and expand the maximum ride length for members

