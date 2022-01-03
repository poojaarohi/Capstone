# Tennesseans without health insurance
## MOTIVATION

This project is intended to demonstrate the factors affecting health care coverage in Tennessee. Coming from a healthcare claims background I was interested to analyze the trend in the health insurance coverage and its impact on general population. Data used for this analysis will be Uninsured population per County in TN, Median Household Income, Uninsured Population by Race/Ethnicity, Age and Gender.  I explored the following:

•	What are the top 10 counties and bottom 10 Counties in the TN with respect to the uninsured population? How have these numbers changed, if at all, over that decade?

•	Relationship between the Median Household Income of TN from 2010-2020 and Uninsured population and find any correlation if any.

•	Who are the uninsured population in TN based on Race/Ethnicity, Age and Gender Distribution and how it has changed over the decade.


## DATA

To answer these questions, I used Census.gov data provided by the Small Area Health Insurance Estimates (SAHIE) over the years 2010-2019.This Data contains the health insurance coverage in the United States. However for my project I have downloaded Data for Tennessee state only. Data Contains distribution by County, Race/ethnicity, Age.


## ANALYTICAL APPROACH

Known  Issues and Challenges:

•	Downloading Data thru API: Access to the data was only thru API with multi-layer variables. And some of the variables were not available in consistently within the data sets.I have written a code using loop function in python to download data for each year and then combined it together to form a data frame from year 2010-2019. I encountered Multiple time outs when the search criteria was retrieving too much data. Hence analysis was required to limit the search criteria

•	Plotting TN County in Tableau: To plot this map I had to download FIPS codes for each county and merge that with the census data.


## TOOLS USED

•	Excel – Data downloaded was in separate workbooks, which were cleaned and merged in Python.

•	Python/Pandas – API for downloading Data from Census.gov and for exploration and aggregation of the data.

•	Tableau - for creating interactive dashboard

•	Git for version control


## SOURCE

https://www.census.gov/library/publications/2020/demo/p60-271.html

https://www-statista-com.proxyiub.uits.iu.edu/statistics/206008/median-household-income-in-tennessee/>


## TABLEAU STORY
Please follow this link to see my analysis and conclusions in Tableau Story format. This Story is stored on Tableau Public. 
