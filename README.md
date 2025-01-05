# Case-study-Bike-share- Google Data Analytics Capstone
Course: [Google Data Analytics](https://www.coursera.org/learn/google-data-analytics-capstone)

## Introduction 
In this case study, I am a junior data analyst for the marketing analyst team at Cyclistic, a bike-share company in chicago. In order to answer the buenisses marketing questions, I will follow the process steps of data analysis: Ask, Prepare, Process, Analyze, Share, and Act. 

### Links
Data Source: [Divvy_tripdate](https://divvy-tripdata.s3.amazonaws.com/index.html)
1. [Data-combining](Data-combining)
2. [Data Analysis](https://github.com/BTiffee/Case-study-Bike-share/blob/161b526fbdefc122bcd339883484f7450934f46f/Data%20Analysis)
3. [Data Visuals]()

## Background
In 2016, Cyclistic launched a successful bike-share o ering. Since then, the program has grown
 to a eetof5,824bicycles that are geotracked and locked into a network of 692 stations
 across Chicago. The bikes can be unlocked from one station and returned to any other station
 in the system anytime.
 Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to
 broad consumer segments. Oneapproach that helped make these things possible was the
 exibility of its pricing plans: single-ride passes, fu l-day passes, and annual memberships.
 Customers whopurchase single-ride or ful-day passes are referred to as casual riders.
 Customers whopurchase annual memberships are Cyclistic members.
 Cyclistic’s nance analysts have concluded that annual members are much more pro table
 than casual riders. Although the pricing exibility helps Cyclistic a ract more customers,
 Morenobelieves that maximizing the number of annual members wil be key to future growth.
 Rather than creating a marketing campaign that targets al-new customers, Moreno believes
 there is a solid opportunity to convert casual riders into members. She notes that casual riders
 are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.
 Morenohasset aclear goal: Design marketing strategies aimed at converting casual riders into
 annual members. In order to do that, however, the team needs to be er understand how
 annual members andcasual riders di er, why casual riders would buy a membership, and how
 digital media could a ect their marketing tactics. Moreno and her team are interested in
 analyzing the Cyclistic historical bike trip data to identify trends.

 ## Scenario
I assume I am a junior data analyst on the marketing analytics team at Cyclistic, a bike-share company based in Chicago. The director of marketing believes that the company’s future success depends on increasing the number of annual memberships. To support this goal, your team seeks to understand the differences in how casual riders and annual members use Cyclistic bikes. These insights will inform the development of a new marketing strategy aimed at converting casual riders into annual members. Before moving forward, however, Cyclistic executives must approve your recommendations, which need to be supported by compelling data insights and professional data visualizations.

# Ask
Three key questions will guide the future marketing program:

1. How do annual members and casual riders use Cyclistic bikes differently?
2. What motivates casual riders to purchase Cyclistic annual memberships?
3. How can Cyclistic leverage digital media to encourage casual riders to become members?

# Prepare
## Data Source
I will analyze Cyclistic trip data to identify trends from January 2023 to December 2023. This publicly available data allows us to explore how different customer types use Cyclistic bikes. However, due to data privacy regulations, personally identifiable information is excluded. This means we cannot link past purchases to credit card numbers to determine if casual riders live within the Cyclistic service area or if they have purchased multiple single passes.

There are 12 files with naming convention of YYYYMM-divvy-tripdata and each file includes information for one month, such as the ride id, bike type, start time, end time, start station, end station, start location, end location, and whether the rider is a member or not. The corresponding column names are ride_id, rideable_type, started_at, ended_at, start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat, end_lng and member_casual.

# Process
Bigquery was used for this data analysis, due to the large datasets. 
A worksheet can only have 1,048,576 rows in Microsoft Excel because of its inability to manage large amounts of data. Because the Cyclistic dataset has more than 4.8 million rows, it is essential to use a platform like BigQuery that supports huge volumes of data.
4844349

# Combining the Data
SQL Query: [Data Combining](Data-combining)
I combined 8 CSV files as tables in the Bigquery labled "case-study-446717.202301_Divvy.2023_Results", the other 4 CSV files were combined in a seperate talbe due to not having the same format labled "case-study-446717.202301_Divvy.2023_Results_summer" creating 4,844,349 rows of data for the entire year. 

# Data Analyze and Share 
SQL Query: [Data Analyze](https://github.com/BTiffee/Case-study-Bike-share/blob/161b526fbdefc122bcd339883484f7450934f46f/Data%20Analysis)
The analysis question is: How do annual members and casual riders use Cyclistic bikes differently?

