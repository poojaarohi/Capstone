# Tennesseans without health insurance
## MOTIVATION

This project is intended to demonstrate the factors affecting health care coverage in Tennessee. Coming from a healthcare claims background I was interested to analyze the trend in the health insurance coverage and its impact on general population. Data used for this analysis will be Uninsured population per County in TN, Median Household Income, Uninsured Population by Race/Ethnicity, Age and Gender.  I explored the following:

•	What are the top 10 counties and bottom 10 Counties in the TN with respect to the uninsured population? How have these numbers changed, if at all, over that decade?

•	Relationship between the Median Household Income of TN from 2010-2020 and Uninsured population and find any correlation if any.

•	Who are the uninsured population in TN based on Race/Ethnicity, Age and Gender Distribution and how it has changed over the decade.


## DATA

To answer these questions, I used Census.gov data provided by the Small Area Health Insurance Estimates (SAHIE) over the years 2010-2019.This Data contains the health insurance coverage in the United States. However for my project I have downloaded Data for Tennessee state only. Data Contains distribution by County, Race/ethnicity, Age.



## ANALYTICAL APPROACH

<b>Known  Issues and Challenges:</b>

•	Downloading Data thru API: Access to the data was only thru API with multi-layer variables. And some of the variables were not available in consistently within the data sets.I have written a code using loop function in python to download data for each year and then combined it together to form a data frame from year 2010-2019. I encountered Multiple time outs when the search criteria was retrieving too much data. Hence analysis was required to limit the search criteria

![API code](https://user-images.githubusercontent.com/90284853/147978642-db0e36cf-00fe-4dd3-8b54-0cc2e1927e3c.jpeg)


![API code2](https://user-images.githubusercontent.com/90284853/147978742-f2176124-3bab-4faf-8175-5801aaf2b80c.jpeg)

•	Plotting TN County in Tableau: To plot this map I had to download FIPS codes for each county and merge that with the census data.


![Screenshot 2022-01-03 145108](https://user-images.githubusercontent.com/90284853/147979084-a415da00-1a13-40d9-81ce-1f08286ad837.png)

Most insured counties are clubbed around Middle Tennessee whereas most uninsured counties stretch toward east TN. 
	One of the factors that can explain this is the difference in the type of couties i.e. Rural/Self Employed v/s corporates (which provide insurance to employees)
  the top 5 insured counties were 

- Williamson (6.28)
-Montgomery (9.34)
-Wilson (9.50)
-Moore (10.20)
-Sumner (10.35)


![Screenshot 2022-01-03 144943](https://user-images.githubusercontent.com/90284853/147979044-4ff2d578-482a-4666-b167-0f0b6e8c0754.png)

In an effort to analyze the vast difference of uninsured counties, I analyzed at a higher level i.e. Median Household income and Unisured population 	for TN.
 Median Household income has grown steadily by 30% between 2013 and 2017, during the same time uninsured population has dropped by 6%. 
	Affordable care act played the major role in this decline.
	Income was not the factor for people shying away from insurance as the income is still on an upward trajectory as well as uninsured population. 
	One explanation of this is the repealing of the individual mandate in 2017.The Affordable Care Act’s individual mandate requires most Americans to enroll in health insurance. In 2017, Congress eliminated financial penalties associated with failing to comply with the mandate.

![Screenshot 2022-01-03 145445](https://user-images.githubusercontent.com/90284853/147979471-fbf92179-3e9b-427c-b9bb-908c4bb757a2.png)

Further I have analyzed the uninsured population by demographics to find any consistency or trend. 
	Over the years, African-Americans and Hispanic uninsured population has not changed significantly. 
	We see the a huge dip in White uninsured population between 2013 to 2016, 
		if we take this data point to age based analysis we can see 19-39 year population has seen the most movement. 
	Gender based categorization tells us the male population is leading this statistics. Also i was surprised to see that the trends for both male and female follwed the same pattern.
	Hence combining these trends we can tell White Male between 19-39 years of age are most uninsured.
![Screenshot 2022-01-03 145503](https://user-images.githubusercontent.com/90284853/147979521-6750faf2-4786-4adc-a1b9-4a570506bb80.png)


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
