# Hypothesis-testing

In this project I test the following hypothesis: university towns in the US have their mean housing prices
less effected by recessions. I run a t-test to compare the ratio of the mean price of houses in university
towns the quarter before the recession starts compared to the recession bottom. 
(price_ratio=quarter_before_recession/recession_bottom)

This project is one of the assignments in the course "Introduction to Data Science in Python" on Coursera
provided by University of Michigan.

Definitions:

A _quarter_ is a specific three month period, Q1 is January through March, Q2 is April through June, 
Q3 is July through September, Q4 is October through December.

A _recession_ is defined as starting with two consecutive quarters of GDP decline,
and ending with two consecutive quarters of GDP growth.

A _recession bottom_ is the quarter within a recession which had the lowest GDP.

A _university town_ is a city which has a high percentage of university students compared to the total 
population of the city.

The following data files are used:
From the Zillow research data site there is housing data for the United States. In particular the datafile 
for all homes at a city level, City_Zhvi_AllHomes.csv, has median home sale prices at a fine grained level.
From the Wikipedia page on college towns is a list of university towns in the United States which has been 
copy and pasted into the file university_towns.txt.
From Bureau of Economic Analysis, US Department of Commerce, the GDP over time of the United States 
in current dollars (chained value in 2009 dollars), in quarterly intervals, in the file gdplev.xls. 

For this project, I only look at GDP data from the first quarter of 2000 onward.
