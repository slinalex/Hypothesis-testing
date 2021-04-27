# Hypothesis testing

In this project I test the following hypothesis: university towns in the US have their mean housing prices less effected by recessions. 

Let m1 = PriceRatioUni = (mean housing prices in university towns the quarter before recession)/(mean housing prices in university towns at recession bottom).
Let m2 = PriceRatioUS = (mean housing prices in the US the quarter before recession)/(mean housing prices in the US at recession bottom).

Null hypothesis: m1 $\geq$ m2

Alternative hypothesis: m1 $<$ m2

This project is one of the assignments in the course "Introduction to Data Science in Python" on Coursera provided by University of Michigan.

Definitions:
- A _quarter_ is a specific three month period, Q1 is January through March, Q2 is April through June, Q3 is July through September, Q4 is October through December.
- A _recession_ is defined as starting with two consecutive quarters of GDP decline, and ending with two consecutive quarters of GDP growth.
- A _recession bottom_ is the quarter within a recession which had the lowest GDP.
- A _university town_ is a city which has a high percentage of university students compared to the total population of the city.

The following data files are used:
- From the [Zillow research data site](http://www.zillow.com/research/data/) there is housing data for the United States. In particular the datafile for [all homes at a city level](http://files.zillowstatic.com/research/public/City/City_Zhvi_AllHomes.csv), ```City_Zhvi_AllHomes.csv```, has median home sale prices at a fine grained level.
- From the Wikipedia page on college towns is a list of [university towns in the United States](https://en.wikipedia.org/wiki/List_of_college_towns#College_towns_in_the_United_States) which has been copy and pasted into the file ```university_towns.txt```.
- From Bureau of Economic Analysis, US Department of Commerce, the [GDP over time](http://www.bea.gov/national/index.htm#gdp) of the United States in current dollars (chained value in 2009 dollars), in quarterly intervals, in the file ```gdplev.xls```. For this project, I only look at GDP data from the first quarter of 2000 onward.
