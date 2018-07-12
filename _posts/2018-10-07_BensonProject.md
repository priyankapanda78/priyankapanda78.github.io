---
## Benson Project

### Introduction
We were off to a good start on our first day at Metis. At the end of the day our project was introduced. As the heading suggests the project name was Benson! Why the name Benson? I will get back on this. Our cohort was divided in groups of four. Each team was tasked to do a presentation on the data analysis findings by the end of week. Problem statement was to recommend subway stations for WTWY(Women Tech Women Yes) Gala street team to solicit at and create awareness in New York. The street team would reach out people for attending the gala and donate for the cause. MTA data is to be used for this analysis.

### Approach
We started brainstorming and came up with various ideas for approaching this problem. After considering different additional data sources like census, Yelp, Google maps API we finalized to add data from census (ACS). The census data has various data points to consider like the household income, demographic, location near to MTA stations.The median income of New Yorkers who are likely to attend the WTWY Gala and contribute is 150K to 200K according to our assumption. The income brackets with more than 200K are less likely to use MTA subway stations and the income with less than 150K are less likely to attend the Gala. Also the income range for people in tech varies between 150K to 200K. Our aim was to maximize the audience for this Gala where the MTA stations are located with the target population.
The MTA turnstile data is available weekly for the subway stations. To analyze the MTA turnstile data for 2018 we have decided to take the morning entries data from 6AM to 1PM for months February 2018 to June 2018. We also assumed higher number of turnstile entries data in the morning as most people commute to work or their destination from their house in this time range.

### Analysis
Exploratory data analysis is performed on the census and MTA turnstile data. The census data is filtered by 150K-200K household income with their respective zip code and the total percentage of people with this income range for a zip code was calculated. The % of people with this income range we can see in this table below.

![p1]({{ site.url }}/public/benson/P1.png)

The zip code for MTA stations were derived with the help of Googlemap Geocoder API and the census data is merged by the zip code. The % of people with income is then multiplied with the daily morning entries data for each subway station to get the total number of people. And these are the top performing 10 stations with the highest footfall in the specified range.

![topStations]({{ site.url }}/public/benson/topStations.png)

### Results
As we can see the top 10 stations based on the income bracket, we would like to recommend the top 3 stations out of them for the street team to solicit for WTWY Gala i.e.
1. 34th Penn Station
2. Grand Central - 42 Street        
3. 42 St - Port Authority


![p3]({{ site.url }}/public/benson/p3.png)

-----





