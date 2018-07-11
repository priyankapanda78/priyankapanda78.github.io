---
## Benson Project

### Introduction
The first day at Metis off to a good start and by the end of the day project was introduced. As the heading suggests the project name was Benson! Why the name Benson? I will get back to you on this. We were all divided in groups of four and as a team by the end of week do a presentation on the data analysis findings. The problem statement was with the help of MTA data, recommend subway stations for the street team to solicit for WTWY Gala(Women Tech Women Yes Gala) and create awareness in New York. The street team have to reach out people who can attend gala and donate for the cause.

### Approach
We started brainstorming and came up with various ideas how to approach this problem. After considering different additional data sources like census, Yelp, Google maps API we finalized to add data from census (ACS). The census data has various data points to consider like the house hold income, demographic, location near to MTA stations.The median income of New Yorkers who are likely to attend the WTWY Gala and contribute is 150K to 200K according to our assumption. The income brackets with more than 200K are less likely to use MTA subway stations and the income with less than 150K are less likely to attend the Gala. Also the income range for people in tech varies between 150K to 200K. Our aim was to maximize the audience for this Gala where the MTA stations are located with the target population.
The MTA turnstile data are available weekly wise for the subway stations. To analyze the MTA turnstile data for 2018 we have decided to take the morning entries data from 6AM to 1PM for months February 2018 to June 2018. We were assuming higher number of turnstile entries data in the morning as most people commute to work or their destination from their house in this time range.

### Analysis
Exploratory data analysis is performed on the census and MTA turnstile data. The census data is filtered by 150K-200K household income with their respective zip code and the total percentage of people with this income range for a zip code is calculated. The % of people with this income we can in this table below.
The zip code for MTA stations were derived with the help of Googlemap Geocoder API and the census data is merged by the zip code. The % of people with income is then multiplied with the daily morning entries data for each subway station to get the total number of people. And these are the top performing 10 stations with the highest footfall in the specified range.


### Results
As we can see the top 10 stations based on the income bracket, we would like to recommend the top 3 stations out of them for the street team to solicit for WTWY Gala i.e.
1. 34th Penn Station
2. Grand Central - 42 Street
3. 42 St - Port Authority



