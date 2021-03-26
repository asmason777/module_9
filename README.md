# Surfs Up Analysis
---
## Overview of Project

### Purpose

Before investing in a surf and shake shop on the island of Oahu, investor W. Avy would like to review weather analytics near the proposed location, specifically temperatures. Two months, June and December, were chosen to represent both summer and winter weather patterns on the island. 

## Results

### Methodology

Weather data from 9 different weather stations on the island of Oahu spanning from 2010 through 2017 were available via an SQLite database file. In Python, SQLite files can be queried using a tool known as SQLalchemy ultimately making it possible to filter data in databases without having to utilize a database software such as SQL. 

Using a query, it was possible to pull the temperature measurements at all nine stations for both June and December from the data file which spanned from January 2010 through August 2017 (in total eight years of June and 7 years of December measurements). Once that data had been converted into a table (data frame), it was then easy to use the describe function to gather the summary statistics for both months. 

### Tables
 
[![June-Temp-Stats.png](https://i.postimg.cc/3xtmQ3h3/June-Temp-Stats.png)](https://postimg.cc/VJbdjQ5h)  “                    “[![Dec-Temp-Stats.png](https://i.postimg.cc/8cGjrYGy/Dec-Temp-Stats.png)](https://postimg.cc/8Jy12tjW)  

### Table Observations

* The average temperatures for both June and December are as expected with June being slightly warmer, 75 to 71, respectively.
  
* The standard deviations are also very comparable (3.25 in June compared to 3.75 in December) meaning that both months tend to have very similar weather patterns.   
 
* Both have comparable record highs (85 for June and 83 for December) but December’s lowest reading comes in at 56 while June is warmer at 64.  

## Summary

Based on temperatures alone, it appears that the while June is hotter by an average of about four degree Fahrenheit, temperatures appear to remain relatively consistent in both months. And although December is cooler and thus more likely to have “cold days”, it is doubtful that this would be a major cause for concern as far as attracting customers as the winter months consistently attract large number of tourists escaping much colder weather elsewhere. 

While temperatures provide one metric by which to measure the popularity of potential customers wanting to surf and/or buy ice-cream based goodies, another important metric to analyze would be rainfall. Rainy days, more than temperature, may impact the number of tourists and locals that visit the beach. Thus, the following two queries would potentially provide more apt information:

1)	Number of days with precipitation per month. 

2)	Number of days with an elevated amount of precipitation per month.

Using these two metrics would help W. Avy determine how many “down” sales days his shop might expect. Likely a small amount of rain would not affect crowds at the beach but on days or times of the year that experience heavy rainfall, it would be necessary to include these calculations when determining future profitability. 
