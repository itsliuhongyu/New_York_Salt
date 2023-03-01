# Salty New York

# What is this?

This is a project analyzing the relationship between snowfall in the New York City and the salinity of the Bronx River.

# Gather the data

This project is a combination several datasets provided by multiple agencies:

1. DSNY Salt Usage:

DSNY report their dispense of salt in the city on [NYC Open Data](https://data.cityofnewyork.us/City-Government/DSNY-Salt-Usage/tavr-zknk). 

2. Bronx River salinity data:

[USGS](https://data.cityofnewyork.us/City-Government/DSNY-Salt-Usage/tavr-zknk) has a monitoring site at the New York Botanical Garden. The site started monitoring the water salinity since 2021. All USGS is in RDB format. Using Python, I managed to scrape the database as string and convert it into a csv so that pandas can read it.

3. Snowfall data at the Central Park:

[NOAA](https://www.ncdc.noaa.gov/) has a weather information database available upon request. I chose the monitoring site located at the Central Park of NYC, and asked for all the snowfall data from Jan.1, 2016.

Special thanks to Dr. Smith from the USGS for sending me additional background information about the Bronx River.

# Analyze Data

1. Analyze the snowfall and river salinity data

Due to the limit that the river salinity data only begins from June 2021, I used a line chart to plot the change of the river salinity through time. I noticed a obvious peak in salinity around Jan. 2022, so I decided to compare the chart with the snowfall data. I used measuring snow on the ground because I want to show how much snow have melt as the melting water might carry salt into the river. 

2. Analyze the relationships between snowfall and salt use

Using separate bar plots, I showed the total tons of salt deployed and the inches of snow fall in each season. Then, I created a separate plot of the tons of salt for each inches of snow.

# What can be improved?

The analysis is no where scientific nor comprehensive, as there are only two years of the salinity data included. I tried to look for other adjacent sites instead, but could not find another good matches. I also hope to directly compare the tons of salt deployed with the river salinity, especially the tons of salt deployed approximate to the river.
