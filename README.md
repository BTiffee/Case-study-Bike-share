# Case-study-Bike-share- Google Data Analytics Capstone
Course: [Google Data Analytics](https://www.coursera.org/learn/google-data-analytics-capstone)

## Introduction
In this case study, I am a junior data analyst for the marketing analysis team at Cyclistic, a bike-share company in Chicago. In order to answer the business marketing questions, I will follow the steps of the data analysis process: Ask, Prepare, Process, Analyze, Share, and Act.

### Links
Data Source: [Divvy_tripdate](https://divvy-tripdata.s3.amazonaws.com/index.html)
1. [Data-combining](Data-combining)
2. [Data Analysis](https://github.com/BTiffee/Case-study-Bike-share/blob/161b526fbdefc122bcd339883484f7450934f46f/Data%20Analysis)
3. [Data Visuals](https://public.tableau.com/views/CaseStudy-BikeShare_17360392452470/Sheet2?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Background

In 2016, Cyclistic launched a successful bike-share program. Since then, the program has expanded to a fleet of 5,824 bicycles, all geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked at one station and returned to any other station in the system at any time.

Until now, Cyclistic’s marketing strategy has focused on building general awareness and appealing to broad consumer segments. A key factor behind this success has been the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as "casual riders," while those who buy annual memberships are known as "Cyclistic members."

Cyclistic’s financial analysts have determined that annual members are significantly more profitable than casual riders. While the flexible pricing plans have helped attract a wide customer base, Marketing Director Moreno believes that increasing the number of annual members will be crucial for future growth. Instead of focusing solely on attracting new customers, Moreno sees a strong opportunity to convert casual riders into members. After all, casual riders are already familiar with the Cyclistic program and have chosen it for their transportation needs.

Moreno has set a clear goal: to design marketing strategies aimed at converting casual riders into annual members. To achieve this, however, the team needs to better understand how annual members and casual riders differ, why casual riders would choose to purchase a membership, and how digital media could influence their marketing efforts. To gain these insights, Moreno and her team plan to analyze Cyclistic’s historical bike trip data to identify relevant trends.

 ## Scenario

I am a junior data analyst on the marketing analytics team at Cyclistic, a bike-share company based in Chicago. The director of marketing believes that the company’s future success hinges on increasing the number of annual memberships. To support this goal, our team is working to understand the differences in how casual riders and annual members use Cyclistic bikes. These insights will guide the development of a new marketing strategy focused on converting casual riders into annual members.

Before moving forward, however, our recommendations must be approved by Cyclistic executives. These recommendations will need to be supported by compelling data insights and professional data visualizations.

# Ask

Three key questions will guide the development of the future marketing program:

How do annual members and casual riders use Cyclistic bikes differently?
What motivates casual riders to purchase Cyclistic annual memberships?
How can Cyclistic leverage digital media to encourage casual riders to become members?

# Prepare
## Data Source

I will analyze Cyclistic trip data to identify trends from January 2023 to December 2023. This publicly available data allows us to explore how different customer types use Cyclistic bikes. However, due to data privacy regulations, personally identifiable information is excluded. This means we cannot link past purchases to credit card numbers or determine if casual riders live within the Cyclistic service area, nor can we identify if they have purchased multiple single-ride passes.

There are 12 files, each following the naming convention of YYYYMM-divvy-tripdata, with one file for each month. Each file includes information such as the ride ID, bike type, start time, end time, start station, end station, start location, end location, and whether the rider is a member or not. The corresponding column names are ride_id, rideable_type, started_at, ended_at, start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat, end_lng, and member_casual.

# Process

BigQuery was used for this data analysis due to the large size of the datasets. A worksheet in Microsoft Excel can only handle 1,048,576 rows, making it unsuitable for managing large amounts of data. Since the Cyclistic dataset contains more than 4.8 million rows, it is essential to use a platform like BigQuery, which is designed to support large volumes of data.

# Combining the Data
SQL Query: [Data Combining](Data-combining)
I combined 8 CSV files as tables in BigQuery, labeled "case-study-446717.202301_Divvy.2023_Results". The remaining 4 CSV files were combined into a separate table due to format differences, labeled "case-study-446717.202301_Divvy.2023_Results_summer". This resulted in a total of 4,844,349 rows of data for the entire year.

# Data Analyze and Share 
SQL Query: [Data Analyze](https://github.com/BTiffee/Case-study-Bike-share/blob/161b526fbdefc122bcd339883484f7450934f46f/Data%20Analysis)
Data Visualization: [Tableau](https://public.tableau.com/views/CaseStudy-BikeShare_17360392452470/Sheet2?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

The analysis question is: How do annual members and casual riders use Cyclistic bikes differently?
To start off the analyis I wanted to determine the bike types between users. 
<picture><![Bike Types](https://github.com/user-attachments/assets/47fd748b-adb4-45fe-931c-27220acbe373)>

I developed a hypotheses that the casual riders may be tuorist visiing chicago during tourist months. 
<picture><![Month per Riders (1)](https://github.com/user-attachments/assets/b6653f64-4b50-4f81-a6f0-a479f74626af)>


Than I wanted to break up the days of the week to see if there are any trends with the causal riders.
<picture><![Average day per riders](https://github.com/user-attachments/assets/897a4091-966d-4398-8c8d-43e7158ac058)>




I wanted to check if there is a time that causal riders are greater than member riders
<picture><![Average per day Riders (2)](https://github.com/user-attachments/assets/c694a554-05d9-489e-813a-093a95783c73)>








