# da1-capstone-medical-debt

## da1-capstone-medical-debt

## Overview

This is a project to explore medical debt in collections and its correlates in the state of Kentucky, my home state. As the 5th poorest state in the nation as of 2017, (https://www.kentucky.com/news/health-and-medicine/article233354582.html) it is worth exploring the burden of medical debt on the population of this state. Look at medical debt in collections by county. I am looking at both the median amount of medical debt in collections by county and the percent of the county with medical debt in collections. I am assuming that medical debt sent to collections is a sign of unmanageable healthcare costs and poor quality insurance, and unemployment/underemployment as health insurance is heavily tied to employment in America. 


The questions:

 - What county characteristics most strongly correlate with medical debt in collections?
	 - at different income levels? (broken down by segments (percentiles)
	 - does bankruptcy rate correlate with medical debt in collections?
	 - is there a relationship between population size of county and medical debt in collections?
 

## Process

Read in data on medical debt, clean it. 
Segment by income level (low income: below 25 percentile, mid income: between 25 and 75 percentile, upper income above 75 percentile).
Merge data with other data.
assess correlations overall
assess correlations within the three income bands.
Analyze the data.
Visualize
Deliverable 
Map percent of medical debt in collections using chloropleth map.

## Sources of data

 - Data from the Urban Institute, which “contains 2016 and 2017 data derived from a random sample of de-identified, consumer-level records from a major credit bureau as well as estimates from summary tables of the US Census Bureau’s American Community Survey (2015 or 2011–15 and 2016 or 2012–16).”
https://apps.urban.org/features/debt-interactive-map/?type=medical&variable=perc_debt_med&state=21

 -2017 population data by county from the Kentucky State Data Center:
http://ksdc.louisville.edu/data-downloads/estimates/
 
Bankruptcy data 2019 by county in KY from US courts:
[https://www.uscourts.gov/statistics/table/f-5a/bankruptcy-filings/2019/09/30](https://www.uscourts.gov/statistics/table/f-5a/bankruptcy-filings/2019/09/30)

## Limitations: 

 - The debt in collections data offers only a snapshot in time: 2017, so I can't look at change through time.
 
 - At the county level, approximately 25% of counties have n/a for median debt in collections. I replaced the n/a's with the median value for all counties, 1295. I did same process for  median medical debt in collections. 
 
 - The bankruptcy data is from 2019, so it does not directly align
 yearwise with the debt in collections data.