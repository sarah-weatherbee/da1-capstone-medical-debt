# Medical Debt in Collections: The Case of Kentucky



## Overview

<p align="center">
<img src="https://user-images.githubusercontent.com/47487494/72007207-c8567500-3216-11ea-8f53-3f7f9cbf9264.jpeg" height="300">
</p>

This is a project to explore medical debt in collections and its correlates in the state of Kentucky, my home state. 
As of 2019, Kentucky had the [sixth highest poverty rate](https://www.usnews.com/news/best-states/slideshows/us-states-with-the-highest-poverty-rates?slide=6)(17%) in the nation. Per 2017 data from the Urban Institute [as noted by the Lexington Herald Leader](https://www.kentucky.com/news/health-and-medicine/article233354582.html), 27 percent of Kentuckians “owe a collection agency for a combined $1.5 billion in recent medical debt"; counties in the eastern pert of the state 
 have the highest rate of people with medical debt in collections. Thus, it is worth exploring the burden of medical debt on the population of this state. I am assuming that medical debt sent to collections is a sign of unmanageable healthcare costs and poor quality health insurance. The proportion of a county with medical debt in collections signals the economic health of a county.


My questions:

* Is health insurance a protective factor against unmanageable medical bills? I.e. medical debt sent to collections?
* Is there a correlation between the number of people with debt in collections and the number of people with medical debt in collections?
* Are people less likely to have debt in collections as income rises?
* Is there a relationship between the percent of people with medical debt in collections and the percent of bankruptcies?


## Process

* Read in data on medical debt in collections, population, bankruptcy to Python Jupyter Notebook
* Clean data 
* Merge datasets
* Assess correlations overall
* Segment by income level (low income: below 25 percentile, mid income: between 25 and 75 percentile, upper income above 75 percentile)
* Assess correlations within the three income bands
* Map percent of medical debt in collections by county using chloropleth map
* Visualize with interactive dashboard in Tableau


## Tableau Dashboard

[Link here](https://public.tableau.com/shared/CW2XM8XZQ?:display_count=y&:origin=viz_share_link)

## Screenshots

<p align="center">
<img src="https://user-images.githubusercontent.com/47487494/72007993-7e6e8e80-3218-11ea-9ba1-3d2a7ef4230d.jpg" height="300">
</p>

<p align="center">
 <img src="https://user-images.githubusercontent.com/47487494/72007471-5cc0d780-3217-11ea-963b-531f5ec47539.jpg" height="400">
</p>


## Sources of data

* Medical debt in collections data from the [Urban Institute](https://apps.urban.org/features/debt-interactive-map/?type=medical&variable=perc_debt_med&state=21)
** This data “contains 2016 and 2017 data derived from a random sample of de-identified, consumer-level records from a major credit bureau as well as estimates from summary tables of the US Census Bureau’s American Community Survey (2015 or 2011–15 and 2016 or 2012–16).”

* County bankruptcy data 2019 by county in KY from [uscourts.gov](https://www.uscourts.gov/statistics-reports/caseload-statistics-data-tables?tn=&pn=All&t=534&m%5Bvalue%5D%5Bmonth%5D=&y%5Bvalue%5D%5Byear%5D=2017)

* County population estimates 2017 from the [Kentucky State Data Center](http://ksdc.louisville.edu/data-downloads/estimates/)


* County boundaries from the [University of Kentucky](https://www.uky.edu/KGS/gis/bounds.htm)


## Limitations: 
  
For counties with missing data, I replaced NaN’s with the median value for that column. 
Median debt in collections NaN’s were replaced with 1295
Median medical debt in collections NaN’s were replaced with 623
Percent of county with medical debt in collections NaN’s were replaced with .29
The debt data is from 2017 while the bankruptcy data is from 2019
The data only offers a snapshot in time; I could not look at how characteristics have changed through the years
